---
title: 'Master Thesis Series: Food Chain Model Equilibria'
date: 2025-06-14
permalink: /posts/2025/06/bifurcation-analysis
tags:
  - blog
  - thesis
---

In this mini-series about topics from my master thesis, I will present some calculations related to my master thesis that did not make into the final thesis.



## Bifurcation Analysis

In my thesis, I am studying a three-species food chain model that exhibits chaos, which was introduced by Hastings and Powell [1].
Here, I present how the nullclines and all equilibria can be calculated in a slightly more complicated model.

$$
\begin{align}
    \dot{u} &= u\cdot (1-\frac{u}{K}) - \frac{\alpha_1 u v}{1 + \beta_1 u} \\
    \dot{v} &= \frac{\alpha_1 uv }{1 + \beta_1 u} - d_vv - \frac{\alpha_2 vw }{1 + \beta_2 v}\\
    \dot{w} &= \frac{\alpha_2 vw }{1 + \beta_2 v} - d_ww
    \label{eq:FC}
\end{align}
$$

One of the first things to do when dealing with any ODE is to identify equilibria and analyse their stability. 

There is one extinction equilibrium, one 1-species equilibrium, one 2-species equilibium and two coexistence equilibria. This calculation is simplified by first calculating the nullclines of the system, which are defined by the zero-manifold of the components.
The manifolds are obtained by setting the individual terms of system \ref{eq:FC} equal to zero.

$$
\begin{align}
1.& \quad du=0 \rightarrow n_1=\{(u,v,w)\in \mathbb{R}^3 | u=0 \}\\
2.& \quad dv=0 \rightarrow n_2=\{(u,v,w)\in \mathbb{R}^3 | v=0 \}\\
3.& \quad dw=0 \rightarrow n_3=\{(u,v,w)\in \mathbb{R}^3 | w=0 \}\\
4.& \quad du=0 \rightarrow n_4=\left\{(u,v,w)\in \mathbb{R}^3 | v=\frac{1}{\alpha_1}\left(1-\frac{u}{K}\right)\left(1+\beta_1u\right) \text{ or } u = \frac{K}{2}-\frac{1}{2\beta_1} \pm \frac{K}{2\beta_1}\sqrt{\left(\beta_1+\frac{1}{K}\right)^2 -\frac{4\beta_1 \alpha_1}{K}v}\right\}\\
5.& \quad dv=0 \rightarrow n_5=\left\{(u,v,w)\in \mathbb{R}^3 | w=\frac{1}{\alpha_2}\left(\frac{\alpha_2u}{1+\beta_1 u} -d_v\right)(1+\beta_2 v) \right\}\\
6.& \quad dw=0 \rightarrow n_6=\left\{(u,v,w)\in \mathbb{R}^3 | v=\frac{d_w}{\alpha_2-\beta_2 d_w} \right\}\\
\end{align}
$$

Equilibria are the points where du, dv, and dw are 0, so intersections of three nullclines for different terms of system \ref{eq:FC}. 
Some of the equilibria are easy to calculate, while others are more complicated.

**Coexistence equilibrium:**
Let's focus on a coexistence equilibrium where all species survive, i.e. for an intersection of $$n_4, n_5$$, and $$ n_6$$.
This is the most complicated case and all other equilibria are easier to calculate.

The nullcline $$n_6$$ determines a value for $$v$$, as we must have

$$v_0=\frac{d_w}{\alpha_2-\beta_2 d_w}.$$

From $$n_4$$, we get

$$\varphi_{u\pm}(v)  = \frac{K}{2}-\frac{1}{2\beta_1} \pm \frac{K}{2\beta_1}\sqrt{(\beta_1+\frac{1}{K})^2 -\frac{4\beta_1 \alpha_1}{K}v}$$

and $$n_5$$ gives

$$\varphi_w(u,v) = \frac{1}{\alpha_2}(\frac{\alpha_2u}{1+\beta_1 u} -d_v)(1+\beta_2 v).$$

There are thus 2 potential coexistence equilibria.
These are obtained by plugging $$v_0$$ into $$\varphi_{u\pm}(v)$$, giving two possible values for $$u$$, $$u_+$$ and $$u_-$$.
Finally, the value of $$w$$ can be calculated by plugging $$v_0$$ and $$u_+$$ or $$u_-$$ into $$\varphi_w(u,v) $$.

All equilibria of the system given by

$$
\begin{align}
    S_0 &= (0,0,0)\\
    S_1 &= (K, 0,0) \\
    S_2 &=\left(\frac{d_v}{\alpha_1 + \beta_1 d_v}, \frac{1}{\alpha_1}\left(1-\frac{d_v}{K(\alpha_1 + \beta_1 d_v)}\right)\left(1+\beta_1 \frac{d_v}{\alpha_1 + \beta_1 d_v}\right), 0\right)\\
    S_3 & =(\varphi_{u+}(v_0),v_0, \varphi_{w}(\varphi_{u+}(v_0),v_0)) \\
    S_4 & =(\varphi_{u-}(v_0),v_0, \varphi_{w}(\varphi_{u-}(v_0),v_0)) \\
\end{align}
$$

It is possible to show that these are indeed all possible equilibria of the system (for which $$u,v$$ and $$w$$ are all non-negative).
Typically, one of the two coexistence equilibria $$S_3$$ and $$S_4$$ also has at least one negative abundance, making it unphysical.

The stability of the equilibria can be calculated by calculating the eigenvalues of the Jacobian of the system at the equilibria. 
While this is straightforward in theory, it entails very tedious calculations with many terms and which is not very insightfull. 
Instead, one can simply use a computer to find the eigenvalues of the Jacobian.


## Bibliography
1. Hastings, A. & Powell, T. Chaos in a Three‐Species Food Chain. Ecology 72, 896–903 (1991).

