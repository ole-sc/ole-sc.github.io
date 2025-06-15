---
title: 'Master Thesis Series: Bifurcation Analysis'
date: 2025-06-14
permalink: /posts/2025/06/bifurcation-analysis
tags:
  - blog
  - thesis
---

I will start a blog miniseries related to my master thesis. In this series, I want to write up early results and studies in an organized way so that I can use them as a template when writing the real thesis.

So far, I am planning to write one post on bifurcation analysis and one on non-autonomous ODEs. We will see if there are additional topics that come up.

## Bifurcation Analysis
We begin with classical bifurcation analysis of autonomous ODEs. I will not write this as a tutorial, but rather as a description of the analysis I am applying to the particular system I am studying.

The system is a three-species food chain model that exhibits chaos [1]
$$\\
\begin{split}
    \dot{u} &= u\cdot (1-\frac{u}{K}) - \frac{\alpha_1 u v}{1 + \beta_1 u} \\
    \dot{v} &= \frac{\alpha_1 uv }{1 + \beta_1 u} - d_vv - \frac{\alpha_2 vw }{1 + \beta_2 v}\\
    \dot{w} &= \frac{\alpha_2 vw }{1 + \beta_2 v} - d_ww
    \label{eq:FC}
\end{split}
\\$$
One of the first things to do when dealing with any ODE is to identify equilibria and analyse their stability. 

There is one extinction equilibrium, one 1-species equilibrium, one 2-species equilibium and a so far unknown number of coexistence equilibria (probably one). This calculation is simplified by first calculating the nullclines of the system, which are defined by the zero-manifold of the components.
The manifolds are
1. $$n_1=\{(u,v,w)\in \mathbb{R} | u=0 \}$$
2. $$n_2=\{(u,v,w)\in \mathbb{R} | v=0 \}$$
3. $$n_3=\{(u,v,w)\in \mathbb{R} | w=0 \}$$
1. $$n_4=\{(u,v,w)\in \mathbb{R} | v=\frac{1}{\alpha_1}(1-\frac{u}{K})(1+\beta_1u)\}$$
1. $$n_5=\{(u,v,w)\in \mathbb{R} | v=\frac{d_w}{\alpha_2-\beta_2 d_w} \}$$
1. $$n_6=\{(u,v,w)\in \mathbb{R} | w=\frac{1}{\alpha_2}(\frac{\alpha_2u}{1+\beta_1 u} -d_v)(1+\beta_2 v) \}$$

$$
\begin{align}
S_0 &= (0,0,0)\\ 
S_1 &= (K, 0,0) \\
S_2 &=\left(\frac{d_v}{\alpha_1 + \beta_1 d_v}, \frac{1}{\alpha_1}\left(1-\frac{d_v}{K(\alpha_1 + \beta_1 d_v)}\right)\left(1+\beta_1 \frac{d_v}{\alpha_1 + \beta_1 d_v}\right), 0\right)\\
S_3 &= \text{TODO}
\end{align}
$$

The coexistence equilibrium (equilirbria) involve even more terms and might be calculated later.
We could go on with a stability analysis, but since the equilibria involve some rather complicated terms, we turn to computational tools to do it for us. 
This can be achieved in the following way: We use the julia package `ForwardDiff` to calculate the Jacobian of the ODE $$\ref{eq:FC}$$, we then plug in the equilibria and calculate the eigenvalues which allows us to programmatically classify the equilibria. 

However, another reason why we are not going through the trouble of calculating the stability of the equilibria is that we are even more interested in the non-equilibrium attractors of the system. 


## Bibliography
1. Hastings, A. & Powell, T. Chaos in a Three‐Species Food Chain. Ecology 72, 896–903 (1991).

