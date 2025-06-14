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

We first calculate the equilibria of this system. There is one extinction equilibrium, one 1-species equilibrium, one 2-species equilibium and a so far unknown number of coexistence equilibria.
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

