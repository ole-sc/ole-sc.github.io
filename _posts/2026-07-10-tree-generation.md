---
title: 'Tree Generation'
date: 2026-07-10
permalink: /posts/2026/07/tree-generation
tags:
  - blog
  - projects
---


Recently, I thought about fun ways of generating trees by recursively adding branches. I have certainly seen very similar approaches in the past, but I can't remember where and what they did exactly. 
This very simple method works quite well in generating nice looking trees and it is also pretty flexible. 
I will also show how to implement this in the programming language Julia.

### Tree Generation
In this approach, a tree is made up of branches in multiple layers.
So far, I only implemented 2D trees, but it would not be hard to extend this to 3D.
A branch has a start point, an end point and a width.

We start with a main branch, usually pointing straight upwards, which is considered to make up layer 1. 

We then recursively add new layers by adding new branches to each branch in the previous layer.
For each layer, we define a rule for how to add the new branches.
For this, we define 
1. the number of new branches
2. The start points of the new branches as a fraction along the previous branch
3. The relative angle of the new branch compared to the previous branch
4. The length of the new branch as a multiplier of the previous branch length.
All of these are collected in a struct `LayerParams`. 




### Example
Below, I show some examples of trees that can be generated with this program. 

<img src='/images/trees/tree2.png'>
The tree below is closely related to the Pythagoras tree, and looks quite cool.
<img src='/images/trees/tree4.png'>
By varying the lengths of the segments, some interesting looking trees can be generated
<img src='/images/trees/tree5.png'>
By adding some randomness into the layer parameters, we can create a large variety of trees. 
One example is the tree below.
<img src='/images/trees/tree6.png'>

