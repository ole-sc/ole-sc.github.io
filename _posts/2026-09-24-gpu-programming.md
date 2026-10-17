---
title: 'GPU Programming'
date: 2026-09-24
permalink: /posts/2026/09/gpu-programming
tags:
  - blog
  - projects
---

### Introduction 
Scientific programming can get computationally expensive very quickly. Usually, it is very easy to increase the amount of calculations arbitrarily. This means that you reach the boundary of what can be computed in a reasonable time relatively quickly.

If the problem is suited, one of the biggest performance increases can be achieved by accessing the parallelization capabilities of the GPU. Learning to use GPUs for scientific computing felt quite difficult to me, partially because there are not so many openly available resources for learning it and because it requires much more thought about data management and task distribution. 

During my master's degree, I learned GPU programming through a couple of different projects. Below, I will show a selection of some of my favorite projects. The projects were created in a game engine called godot. I began implementing some of these projects in julia where gpu programming seems to be a lot easier, but these are not ready to be published yet.

### 1. Mandelbrot Zoom
One of the first projects I made, is a Mandelbrot zoom. This is calculated based on an iterated map. For some complex number $$c$$, we iterate the (complex-valued) map.

$$ z_{n+1} = z_n^2+c$$

We track whether the map stays bounded or if it diverges to infinity as it is iterated many times. By coloring trajectories that escape based on how many iterations it took to diverge, we get the famous Mandelbrot set image. 

Using GPUs, we can make this computation for every pixel in an image very quickly. We can also add a zoom effect and pan around the image, all of which are computed in real-time.  

<img src='/images/shader_experiments/mandelbrot.png'>
<img src='/images/shader_experiments/mandelbrot2.png'>

This uses a fragment shader and is adjusted from a [tutorial](https://docs.godotengine.org/en/stable/tutorials/shaders/your_first_shader/your_first_2d_shader.html) for writing simple fragment shaders.

### 2. Iterated Maps
The mandelbrot set is an example of an iterated map, but there are many other options that we could use. One interesting example is the Henon map. It is a 2D map, which has many interesting properties such as the existence of a chaotic attractor and fractal basin boundaries. But we can actually consider a large set of iterated maps of which the Henon map is just one example.

To this end, we consider the following iterated map:
$$
\begin{align}
    x_{n+1} &= a_1 + a_2 x_n + a_3 y_n + a_4 x_n^2 + a_5 y_n^2 + a_6 x_n y_n\\
    y_{n+1} &= b_1 + b_2 x_n + b_3 y_n + b_4 x_n^2 + b_5 y_n^2 + b_6 x_n y_n
\end{align}
$$

The Henon map has the parameters $$a_1=1, a_3=1, a_4=-1.4$$ and $$b_2=0.3$$ and all other parameters to zero. 
As in the case of the Mandelbrot set, we iterate this map and determine whether it blows up or stays bounded. Each pixel represents a different initial condition in the $$xy$$-plane.
In my implementation, it is possible to change the parameters interactively with the image being updated in real time. 
This kind of problem lends itself very well to GPU computing, because the computation of each pixel is independent of the other pixels and not computationally expensive. Again, the program is based on a fragment shader, which are easy to use in godot.

One thing to note is that fractal boundaries between staying bounded and blowing up are quite common for a large range of parameters. 
Below, you can find some picture for different parameters.

<!-- Obsidian Henon Map note: image1 -> params 5, image2 -> params 6, image 3 -> params 7, image 4 -> params 3 (slightly different) -->
<img src='/images/shader_experiments/iterated1.png'>
<img src='/images/shader_experiments/iterated2.png'>
<img src='/images/shader_experiments/iterated3.png'>
<img src='/images/shader_experiments/iterated4.png'>


### 3. Boids
One of my favorite programs is a simulation of boids.
Boids are an example of complex behaviour emerging from simple rules. 
They were introduced as a simple model of bird flocking and show some fascinating behaviour [1].

The implementation of this simulation was a lot trickier as it required the use of compute shaders, which are not easy to manage in godot. I did learn a lot in the process though. 
I followed this [tutorial](https://www.youtube.com/watch?v=v-xNj4ud0aM) relatively closely for this implementation. 
Using the GPU, I can easily simulate 20000 boids at a good framerate. 

Each boid, which stands for bird-like object, follows three simple rules:
1. Avoid collisions with nearby boids
2. Attemp to match the velocity of nearby boids
3. Attempt to stay close to nearby flockmates

Parameters control the radius of these interaction and the relative strength. The behaviour of the flock changes based on the parameters. 


Below, you can see some screenshots of the simulation. 

<img src='/images/shader_experiments/boids3.png'>
<img src='/images/shader_experiments/boids2.png'>
<img src='/images/shader_experiments/boids.png'>

[1] Reynolds CW. *Flocks, herds and schools: a distributed be-havioral model*. 1987.

<!-- ### Summary

I showed three interesting simulations that I created using GPUs. Much more could be said about the mathematical side of these examples, but . 
In the future, I want to show some more simulations that I created, for example a slime-mould simulation or a visualisation of the Thomas attractor, but which require more work before they can be displayed properly. -->