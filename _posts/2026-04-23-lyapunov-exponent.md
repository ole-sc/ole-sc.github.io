---
title: 'Master Thesis Series: Lyapunov Exponent of the Food Chain Model'
date: 2026-04-23
permalink: /posts/2026/04/lyapunov-exponents
tags:
  - blog
  - thesis
---

One of the nicest results from my master thesis are the figures showing Lyapunov exponents. 

I studied a three-species food chain model with a chaotic attractor. 
In my master's thesis, I used a rescaled version of the model that was described in the previous blog post. 
This model was introduced by Ian McCann and Peter Yodzis who determined biologically plausible parameter values for this model [1].

$$
\begin{align}
    \dot{R} &= r R\cdot (1-\frac{R}{K}) - x_C y_C\frac{R C}{R_0 + R} \\
    \dot{C} &= x_C y_C \frac{RC }{R_0 + R} - x_C C -x_P y_P \frac{ CP }{C_0 + C}\\
    \dot{P} &= x_P y_P\frac{CP }{C_0 + C} - x_P P
    \label{eq:FC}
\end{align}
$$

We consider the system for different values of the parameters $$K$$ and $$y_C$$, while keeping the other parameters constant. 
I used the following parameter values: $$K\in[0.9, 1.05], y_C \in[1.5, 2.5], r=1, R_0=0.161, C_0=0.5, x_C = 0.4, x_P = 0.08,  y_P=2.876$$. 

Lyapunov exponents measure how small volumes of the state space are deformed by the dynamics of the system and allow us to distinguish between different types of attractors. 
Each attractor has a number of Lyapunov exponents that is equal to the dimension of the system, so in our case three. 
When the attractor is chaotic, the largest Lyapunov exponent is positive. 
When the attractor periodic, the largest Lyapunov exponent is zero.
When the attractor is an equilibrium, the largest Lyapunov exponent is negative. 

The Lyapunov exponents are computed for a large number of combinations of different parameter values of $$K$$ and $$y_C$$ and plotted as a heatmap.
This gives us an overview over the dynamics of the system for a large range of parameters, specifically allowing us to identify chaotic parameters.
This figure can be seen below:

<img src='/images/lyapunov/lyapunov_exp_refine2000.png'>

The white parts of the image show for which parameters the base attractor, where all three species coexist, does not exist or is unstable. This corresponds to a "dangerous" bifurcation of the coexistence attractor. 
The dark blue parts of the state space show where the coexistence attractor is periodic. 
Finally, the greenish-yellow parts show chaotic dynamics. 
A fascinating aspect of chaotic systems is the highly complicated structure that the largest Lyapunov exponents show.

There are a lot of interesting aspects to explore, for example the shrimp-shaped periodic parameter regions, the existence of a periodicity hub and regions with multiple coexistence attractors, which I go into more in my master's thesis.
As far as I know, my investigation is the first to show the shrimp-shaped periodic parameter regions in the food chain model.
However, instead of focusing on the mathematical properties, I want to highlight the beauty of these structures here.

In the images below, I removed all axes and colorbars and changed the colormap. Additionally, I changed the figure to show the largest non-zero Lyapunov exponent, which reveals some additional structure in the periodic parameter regions. 
With some finishing touches, we get images that are truly beautiful.



<img src='/images/lyapunov/lyapunov_full_inferno3.png'>

<img src='/images/lyapunov/lyapunov_periodicity_hub_inferno.png'>




## Bibliography
1. McCann, I. & Yodzis, P. *Biological Conditions for Chaos in a Three-Species Food Chain*. 1994. https://doi.org/10.2307/1939558.

