---
title: 'A Paper A Day'
date: 2025-02-04
permalink: /posts/2025/02/a-paper-a-day
tags:
  - project
  - research
---

A paper a day keeps the doctor away... Or was it an apple?

Anyhow, I currently have to choose a topic for my master's thesis and I feel like I could benefit from looking into different research areas to find out what field I want to move into. 
This is one of the reasons that I set myself a challenge: Read one paper every day for a month. 
By reading from a range of topics (of course related to my current interests), I hope to get an idea of different research fields and their open problems and whether I would be interested in pursuing a career in any of these fields.

To keep myself accountable, I set up this blog post, that I will update daily.
Unfortunately, I have some vacation planned, so the project has to paused for a couple of days. 
I want to start now anyways, because I need to decide on a topic relatively soon.

# Project Outline
- Start Date: 4th of February 2025
- Break Time (vacation): 13th - 24th of February
- End Date: 16th of March

Total: 30 Days

**Paper selection:** First, some survey papers from different fields were selected. 
Additionally, some papers related to potential master's thesis topics were included.
Lastly, some papers that just sounded interesting or were written by some of my professors were selected as well.
In total, 15 papers were selected in order to leave room open for follow up research.

**Topics:** I am interested in applying mathematical methods to real problems. Mathematically, I am interested in nonlinear dynamics, network science and statistics. The applications I am generally interested in are climate science, ecology, energy grids, neural dynamics in the brain, urban models and many more though my knowledge about some of these fields is pretty limited.
As you will see, most of the papers listed below will be related to the topics just mentioned.

**Workflow:** Every day, I will post a short summary of the paper and my thoughts on my personal interest in this subject. At the end, I will write a summary of what I learned and new perspectives I gained.

A list of all papers can be found at the bottom of the page.

# Summaries
## 1. Modeling Nonlinear Dynamics and Chaos: A Review (2009)
Aguirre, L. A. & Letellier, C.

**04.02.2025:** 
The paper describes various aspects of building nonlinear models from time series data. The authors shortly introduce early influential works. 
Then, model classes are described that have been used to model nonlinear dynamics like polynomials, neural networks, radial basis functions, wavelets and more.
Structure selection, or the question of choosing a model that is as simple as possible but sufficiently complex to capture the dynamics underlying the data, and embeddings as part of the modeling process are discussed.
Lastly, techniques for parameter estimation and model validation were described.

In summary, most aspects of model construction from time series data were discussed and examples of papers were provided. Though likely being out-of-date, it might serve as a really good reference work for finding previous work in this area. From here it would be interesting to see whether there are more recent papers along the lines of this one.
Though this direction of research is interesting to me, I am more interested in understanding a given ODE rather than finding an ODE that describes some given data well. 

## 2. 25 years of criticality in neuroscience — established results, open controversies, novel concepts (2019)
Wilting, J. & Priesemann, V.

**05.02.2025:** In the paper the controveries behind the concept of criticality in the brain is discussed: Power law distibutions of avalanches, that is cascades of neural activity, were found in experiments suggesting neural activity is in a critical state. However, follow-up, in vivo experiments usually do not show power law distributions of avalanche sizes.
Criticality would leat to some positive and some negative effects to brain function. The authors argue that the best balance between these effects is likely achieved close to, but not exactly at criticality. 
Based on a previous publication by the authors where they introduced a method to quantify the distance to criticality, they argue that the brain is in a "reverberating regime" that has some upsides and can potentially resolve the controversities surrounding criticality.

Short and easy to read. Gives an interesting overview of the question of criticality and offers a potential solution. The topic is very fascinating and I could certainly see myself moving in this direction at some point. I will add another paper related to this topic, because I feel like a lot of aspects of computational neuroscience are not covered.

## 3. Atlantic overturning inferred from air-sea heat fluxes indicates no decline since the 1960s (2025)
Terhaar, J., Vogt, L. & Foukal, N. P.

**06.02.2025:** The authors argue that the subpolar gyre (SG) sea surface temperature (SST) is not as good a proxy as previously assumed.
Based on CMIP6 models, the authors find a strong relation between air-sea heat flux anomalies and AMOC anomalies and propose this as a better proxy. They reconstruct the AMOC strength based on air-sea heat flux observations since 1958 and find no indication of decline.
They also state the variability of the reconstructed AMOC anomaly is lower than in climate models suggesting that climate models underestimate the AMOC stability.

A couple of weeks ago, I presented a paper warning about a collapse of the AMOC by Ditlevsen and Ditlevsen. Their prediction was based on the SG SST and this paper suggests that this proxy might not have been as good as assumed (among some other problems).
I think to really judge the methods, a better understanding of the CMIP models is necessary. I would be interested in staying up to date in the ongoing discussion about the AMOC. 
I am not sure whether I could contribute in a meaningful way to the AMOC research in the future because it is already so actively researched and discussed.


## 4. Adaptive coevolutionary networks: a review (2008)
Gross, T. & Blasius, B.

**07.02.2025:** Adaptive networks combine dynamics of the node states and dynamics of the network topology. 
They occur in a large variety of scenarios like: social networks, neural networks, game theory, infrastructure and more. A variety of mostly conceptual models is reviewed. These models are based on either rewiring links or changing weights usually based on local rules. Among the observed resulting properties are complex network structure, self-organization to criticality, nodes separating into distinct classes and complex system dynamics. The authors hope to kick off a more extensive investigation of adaptive networks.

I am very interested where the developments of adaptive networks stands today. 
This direction of research is really exciting to me and I am maybe even prefer nonlinear dynamics on networks to a purely nonlinear dynamics focused master's thesis which would build on the papers by Alkhayuon that I will read later in this project.

## 5. Universality in network dynamics (2013)
Barzel, B. & Barabási, A.-L.

**08.02.2025:** The authors derive from some rather general deterministic dynamical equations on networks equations for some important network properties such as local impact and stability, distance-dependent correlation function, and cascade size.
They find that local impact and stability are only influenced by the dynamics and not the topology of the network. 
This results in four universality classes: uniform vs degree-dependent stability and uniform vs degree-dependent impact (four combinations possible.).
For the distance-dependent correlation function (propagation of pertubations) they find either conservative or dissipative dynamics that is governed both by the topology and the dynamics.
For the cascades, the local impact and the propagation determine uniform vs heterogenous cascade sizes.
The authors show that the universality classes can describe the dynamics of four frequently used models very well and predict that these universality classes can be used to study systems with unknown dynamics.

I think the paper was not too difficult to read, though the calculations were outsourced to the supplementary material, and offered an interesting insight into central aspects of network science.
Though very diverse on the surface, the paper predicts that dynamics on networks can be placed into only a few universality classes. I didn't expect to see Laurent expansions again, but they made a reappearence here. 
This suggests that we could also look at dynamics with singularities which I wrote my Bachelor's thesis about and would be interested to study again.
Again, very interesting topic and I will for sure try to further pursue network science in the future.

## 6. Rate-induced tipping from periodic attractors: Partial tipping and connecting orbits (2018)
Alkhayuon, H. M. & Ashwin, P.

**09.02.2025:** This paper discusses nonautonomous nonlinear dynamical systems where a parameter changes at a certain rate, called parameter shift systems.
They show that if the parameter changes from $$\lambda_-$$ to $$\lambda_+$$, there exists a set for a point in time such that if you rewind the clock, you end up at an attractor of the time-independent system with the fixed parameter $$\lambda_-$$.
They show that for an attractor that changes continously in time, then trajectories will stay within the basin of attraction for small rates of change of the parameter.
However, it is possible that some or all trajectories will tip away from this attractor for higher rates of change.
They provide an example that highlights their results and numerically find critical rates of change for this system.

This paper was much more technical than the previous ones and I did not understand everything. 
I read this paper because it is related to one of my potential thesis topics.
The approach is more mathematical than I am used to in my master's degree and I do think that I would like that for my master's thesis.
I am slightly intimidated because there are a lot of things I would have to learn to get a good grasp on this but a lot of these I would also really like to know.

## 7. Towards a comprehensive framework for modeling urban spatial dynamics (2009)
Irwin, E. G., Jayaprakash, C. & Munroe, D. K. 

**10.02.2025:** This paper suggests a framework for modeling urban spatial dynamics as complex adaptive systems.
They argue that a three-stage process should be used: First, identify and monitor key system patterns. 
Then, create simple spatially explicit agent-based models. Lastly, iterate between validating the model and model development.
They argue that defining effective dynamical equations (empirical equations describing the evolution of a observed variable) and comparing them against the effective dynamical equation of the models could help in validation.

The paper did not go into much detail and I would like to see whether their approach has acutally been used succesfully and if their validation method holds up.
Thinking about modeling frameworks is definetly useful for me and I am also interested in modeling cities because they seem to provide a fascinating and important modeling target.
It was cool to see that my skills could be valuable in this area and I am interested to see where the field stands today.

## 8. Inferring collective dynamical states from widely unobserved systems (2018)
Wilting, J. & Priesemann, V.

**11.02.2025:** The authors show that inferring stability using a process with a first order autoregressive representation (PAR) is biased when only a part of the system is observed.
They show that linear regressions have the same bias independent of the number of time steps between observations and use this fact to create an unbiased estimator of the stability.
This means that even very small portions of the network are sufficient to estimate how a close a system is to criticality provided long enough time-series data is available.
The method is used in simulated systems and shown to perfectly predict closeness to criticality while convential methods underestimate it.
They then show that the brain of varying animals is likely very close to, but not exactly at criticality.

The results seem very useful for understanding a variety of systems and much better than previous method.
They seem almost to good to be true, but there are probably limitations why they can't be used absolutely everywhere.
The method does not sound exceptionally complicated so I am surprised it wasn't developed earlier.
I hadn't heard of PAR before and I'd like to understand how it is related to the modeling of complex systems from time-series data as described in the first paper I read.

## 9.  Dynamics of tipping cascades on complex networks (2020)
Krönke, J., et al.

**12.02.2025:** The authors numerically analyse cascades on directed dynamical networks. 
Dynamics on nodes are described by the hysteresis normal form and coupled with adjacent nodes. 
For a variety of different network topologies and properties like networks size and mean degree, they analyse the coupling strength required to lead to large cascades, that is multiple nodes tipping to a different state after a single node tips.
They find that a lower number of nodes and a higher mean degree lead to higher vulnerability.
They also conclude that feed-forward loops have more impact on the vulnerability than feedback loops.

This paper is directly related to the paper about universality classes. The cascade size distributions found here seem to be very different from the universality classes described there.
The ODE equation certainly matches the form preseted by Wilting and Priesemann, so it would be very interesting to calculate the expected results and see whether it matches the observations from this paper.
This paper was very descriptive and did not really try to explain their results mathematically.

## 10.  Phase tipping: how cyclic ecosystems respond to contemporary climate (2021)
Alkhayuon, H., Tyson, R. C. & Wieczorek, S.

**12.02.2025:** For cyclic attractors, it is shown that for the Rosenzweig-MacArthur model and the May model with instant parameter switches, some trajectories can tip to extinction without a bifurcation.
Through the parameter change, a part of the previous limit cycle now lies outside the basin of attraction of the limit cycle with the new parameter value.
A mathematical definition for partial basin instability and phase tipping is put forward.
They show that this explains the simulation results and propose that this is a new tipping mechanism called phase tipping or P-tipping.


To me it seems like this is just rate-induced tipping because the basin of attractions changes as a result of the parameter change which leads to some trajectories leaving the basin of attraction (but I don't know how rate-induced tipping is usually understood.).
This paper was easier to understand than the paper about rate-induced tipping (paper 6) and I like the mathematical approach to studying these systems as it seems more concrete than just qualitatively describing simulation results.
I think that I got a relatively good idea of how one could tackle nonautonomous systems mathematically.

**End of break**

## 11.  Decision-Making in Agent-Based Modeling: A Current Review and Future (2019)
DeAngelis, D. L. & Diaz, S. G.

**25.02.2025:** The paper presents how decision making has been incorporated into mathematical modeling to improve their results.
Some of the decisions are: allocation of time and energy to certain tasks like foraging, reproducing, defending or movement and where to relocate to.
The authors argue that agent-based modeling (ABM) can improve results compared to mathematical models and provide many examples of using ABMs to model ecological systems.
ABMs are able to model individual differences and incomplete knowledge and how this affects population level dynamics.
Recently, genetic algorithms and artificial neural networks have been used which allow agents to evolve decision making strategies over time.

ABM is fascinating and can produce realistic results by being able to model individual interactions. 
However, it seems like the analysis is limited because you just simulate and observe. 
My current studies are not directly connected to ABM, but for some reason this type of simulation really hits the spot for me.
In school, I was interested in game design and ecosystem simulations and I always wanted to program these myself.
Now I understand that it was essentially ABM and that I could even do actual research in that direction if I wanted to.
## 12. The physics of higher-order interactions in complex systems (2021) 
Battiston, F. _et al._ 

**26.02.2025:** In the paper, a short overview of the recent emergence of using higher-order interactions to describe complex systems is given.
While networks are limited to describing pairwise interactions, the authors argue that it is often times more realistic to consider interaction between more than two nodes using hypergraphs or simplicial sets.
There is some evidence to suggest that this is a general pathway towards explosive transitions in networks thus having a strong impact on network dynamics.
The field is in a very early stage of development and many questions like reconstructing higher-order interactions from data are still open.

I think it makes a lot of sense to consider higher-order interations for many systems. 
I am curious whether there might be regular network settings where the dynamics are equivalent to a network with higher-order interaction and simpler dynamical equations.
Overall, the paper could have been a bit more detailed but it provides a lot of interesting further reading options.

## 13.   Can the original equations of a dynamical system be retrieved from observational time series? (2019)
Mangiarotti, S. & Huc, M.

**27.02.2025:** The possibility of reconstructing the dynamical equations underlying chaotic attractors from time series data are analysed. 
They consider 26 low dimensional systems for which they generate multivariate timeseries data. 
Their method of finding dynamical equations is based on narrowing down a large search space of polynomials in multiple steps and preferring less complex results that can still reproduce the observed dynamics.
They find that their method is robust to varying initial values but performance deteriorates when noise is added especially when the systems get more complex.

Interestingly, in these cases it seems to be possible to reconstruct the dynamical equations from the multivariate time series data. 
I expect that the method will become much less accurate for very high dimensional systems, but it seems like the method has potential to work even then or that it could be modified to work in these scenarios.
The paper is directly related to the first paper from this project and where exactly these kinds of approaches were already discussed but apparently not fully developed.

## 14.  Homoclinic bifurcation in a Hodgkin–Huxley model of thermally sensitive neurons. (2000)
Feudel, U. _et al._

**28.02.2025:** Individual thermally sensitive neurons are modeled using a reduced Hodgkin Huxley model. 
The bifurcation diagram of the interspike intervals are shown and a period-doubling cascade to chaos is shown as temperature increases.
Still in the chaotic regime, at some critical temperature some interspike interval times diverge. 
This is identified as a homoclinic orbit of a equilibrium of a saddle-focus type. 
Trajectories move towards the equilibrium along the stable manifold, slowing down before getting ejected along the unstable manifold.
The divergence of return times still exists when a small amountof noise is added, though the other aspects of the chaotic attractor get blurred.
Lastly, in experiments with crayfish cells, a fast increse in interspike intervals was found as well.

I'd like to know if modern neural studies still assume homoclinic orbits exist.
Also, wouldn't this phenomenon also occur with critical slowing down, i.e. a normal type of bifurcation? 
Maybe it does not work in combination with chaos, but if it does, then might this be an example of the reverbarating regime from papers 2 and 8?
For my master topic, I feel like I have a much better intuitive understanding of the phase-tipping concepts.

## 15. Metamorphoses of Basin Boundaries in Nonlinear Dynamical Systems. (1986)
Grebogi, C., Ott, E. & Yorke, J. A.

**01.03.2025:**  This early paper describes how the basin boundary of the Henon map becomes fractal as a bifurcation parameter is changed.
The boundary is given by the stable manifold of a period one saddle point. 
At some point, the stable and unstable manifolds of the saddle point intersect which necessitates an infinite number of crossing leading to a fractal basin boundary.
Through this process, the period-one saddle becomes inaccessible from the basin of attraction of the attractor and a period four saddle becomes accesible.
For another parameter value, the basin boundary suddenly changes size and is accompanied by the period four saddle becoming inaccesible and a preiod three saddle taking its place.
The authors argue that a change in accesibility of unstable orbits mediates a change in the basin boundary.

I think that understanding this example deeply would really help my understanding of nonlinear systems. 
It is also part of the early investigations into nonlinear dynamics and probably what most current experts have learned.
While having understood the general concepts discussed here, how the stable and unstable manifolds interact (and why one crossing necessitates infinitely many crossings) is still not quite clear to me.

## 16. Challenges, tasks, and opportunities in modeling agent-based complex systems. (2021)
An, L. _et al._ 

**02.03.2025:** The history of agent-based modelling (ABM) and their use in different disciplines, as well as challenges and opportunities are discussed.
A variety of challenges is identified such as difficulty regarding coherence in methods and platforms, computational efficiency, transparency and reusability, and generalization of findings.
They discuss the potential of big data to better identify suitable algorithms and the importance of thorough model validation and point to frameworks developed for model description and validation.
Lastly, they point to the potential of using AI to create more realistic agent behaviour.

This is for sure a paper to come back to if I want to use ABM in the future. 
In particular, I want to become able to do thorough model validation to ensure that my results are robust.
Another useful aspect was a pointer to a database of agent-based models.
As stated by the authors as well, one issue I have with ABM is that of generalization, because it is so difficult to tackle them theoretically,
but then again, they seem to be a much more realistic representation of nature and there are apparently validation approaches enabling the identifications of important mechanisms.

## 17.  Homoclinic bifurcation in an ocean circulation box model. (2002)
Kuhlbrodt, T. & Feudel, U

**03.03.2025:** An ocean box model, that was reduced from a slightly more complex model is described and the fixed points and their bifurcations are analysed.
A saddle-node bifurcation and a subcritical Hopf bifurcation are found.
These are caused by two different mechanisms, suggesting that there might be different way the THC could tip.
Additionally, it might be difficult to observe a subcritical bifurcation in simulations.
Lastly, there is a homoclinic bifurcation, when the unstable periodic orbit and the unstable fixed point collide.
The homoclinic loop was calculated numerically.

I have to say, the formatting of this paper was a bit rough. 
The paper can be summarized as calculating the bifurcations in the model.
I think it would be very beneficial to be able to conduct this type of analysis by myself to have a good basis for future research.
I am wondering whether the existance of a Hopf bifurcation is generally accepted for the THC because it is not considered by the Ditlevsen paper.
However, since paper 3 questions the reliability of the data used by Ditlevsen, it might be necessary to redo the analysis with different proxies and potentially consider this Hopf bifurcation as well.

## 18 Network Motifs: Simple Building Blocks of Complex Networks. (2002)
Milo, R. _et al._ 

**04.03.2025:** Network motifs are patterns in real networks occuring with a much higher frequency than in random networks.
The authors implemented an algorithm counting the occurence of 3 and 4 node subgraphs. 
If a given subgraph appeared statistically significantly more often than in a comparable random network, it was flagged as a network motif.
For networks in biochemistry, ecology, engineering and neurobiology motifs were identified. 
It was found that netowrks related to information processing shared similar motifs.
The authors argue that network motifs can define classes of networks that are created by the same elementary principles.

As I have learned in a module that certain motifs allow for determining some eigenvalues easily, I would have liked to learn about more in-depth aspects of network motifs.
However, the results presented here are still very interesting.
It would be interesting if there is something like anti-motifs, that is subgraphs being very uncommon because they impair some of the system functions.

## 19. Tipping points in open systems: bifurcation, noise-induced and rate-dependent examples in the climate system. (2012)
Ashwin, P., Wieczorek, S., Vitolo, R. & Cox, P. 

**05.03.2025:**  A new type of tipping, called rate-induced tipping or R-tipping is introduced. 
Some systems can tip when the rate of change of a parameter exceeds a threshold in a way that is distinct from noise-induced tipping or bifurcation-tipping.
They argue that the effects of a higher dimensional system on a subsystem can be studied by modeling its effect as a time-varying parameter.
The authors develop a criterion for R-tipping that can be used for simple systems but not easy to compute in general. It is not clear how well this approach works in more complicated systems.
In total, 4 systems (normal form of saddle-node and Hopf bifurcation, a fast-slow system and a simple climate model) are studied and it is shown that all of them can exhibit R-tipping and the effects of R-tipping are studied.

I could not understand all of the mathematics in this read-through and there was a lot of maths in this paper but I think I got the main ideas.
I am honestly surprised that the idea of rate-induced tipping is so recent since it seems pretty natural to study systems with changing parameters, but that's easy to say in hindsight.
To me, it seems like almost all systems have time-varying parameters that could potentially lead to R-tipping which means the system is very relevant but potentially understudied.

## 20. Adaptive self-organization in a realistic neural network model. (2009)
Meisel, C. & Gross, T.

**06.03.2025:** A mechanism for self-organised criticality based on adaptive networks is known.
Here, a network with realistic neural dynamics as well as a realisitc update rule for the network links based on the activity of the neurons is simulated.
It is found that the average connectivity evolves to a critical value irrespective of initial connectivity. 
An order measure is found to follow a power law indicating a critical state. 
A variant of the link update rule is used to study the neuron weights. These also follow a power law and are relatively similar to data of human brains, though whether the field data really follow a power law is unclear.
The authors conclude that self-organized criticality is likely in real neural systems.

Adaptive networks are really interesting and seem like a intermediate point between simple mathematical models and ABM, maybe providing a mathematically tractable approach for studying more realistic systems.
This concept of self-organized criticality seems like a very plausible way neural networks might evolve towards criticality and it seems to be possible to reconcile with the idea of a reverberating regime where the brain has mechanism for moving towards cricitality and then perhaps an additional mechanism for avoiding it.

## 21. The Slow Passage through a Hopf Bifurcation: Delay, Memory Effects, and Resonance. (1989) 
Baer, S. M., Erneux, T. & Rinzel, J. 

**07.03.2025:** This paper already considered the effects of a (slowly) time-varying bifurcation parameter on the FitzHugh-Nagumo neuron model. 
Theoretically and analytically, they show that the onset of oscillations in a Hopf bifurcation can both be delayed or accelerated with a varying bifurcation parameter.
They calculate approximations of the moving steady state and its stability and it can be seen that they are qualitatively correct but have some (systematic) errors.
It is found that the delay is related to the initial distance to the steady state bifurcation point, the ramping rate and reduced by noise.

I think it is interesting that time-varying parameters were already studied in 1989 but the concept of rate induced tipping was developed so much later.
I did not manage to follow all of the calculations but it is interesting to see that there are techniques for studying time-dependent solutions and that they are related to fields I am relatively comfortable with (the maths still looks very hard).

## 22. Über die von der molekularkinetischen Theorie der Wärme geforderte Bewegung von in ruhenden Flüssigkeiten suspendierten Teilchen. (1905)
Einstein, A. 

**08.03.2025:** In this paper Albert Einstein argues that osmosis pressure should be present for free particles in a fluid, which is not predicted by classical thermodynamics. 
By considering the free energy of the system, he shows that osmosis pressure is a result of molecular-kinetic theory of heat (which was not established at the time). 
He then shows that a position-dependent force acting on the particles will be cancelled by the osmosis pressure in the stationary state and that this can be viewed as a diffusion process.
The diffusion equation is derived and solved and some predictions are derived, enabling the calculation of the size of the atom.

It was tough summarizing this German paper in English, especially since I am not that familiar with molecular physics, so it is likely not very precise.
However, it was cool reading a paper from the G.O.A.T. himself and interesting to see how much of the maths is familiar and yet slightly different. 
While not being very relevant to my current studies, it never hurts reading up on important historical works.

## 23. “Make no little plans”: Impactful research to solve the next generation of transportation problems. (2021)
Agatz, N., Hewitt, M. & Thomas, B. W.

**09.03.2025:** Based on the UN sustainable development goals (SDG), challenges and research opportunities for the transportation science community are presented. 
The SDG are split into three groups: *well-being, infrastructure and natural environment*. 
Some of the areas discussed are access to health care, improving public transport and other alternatives to car transport in cities, and responding to natural disasters. Reducing CO2 emissions was not discussed in detail.
Some of the general areas requiring more developments are multi-objective modeling, modeling under uncertainty and integrating stakeholder behavior into models.
To achieve good results, the authors call on researchers to engage more with stakeholders and focus more on solving relevant problems than publishing in journals. Additionally, the importance of interpretability of models and results is emphasized to improve the likelihood of implementation.

While not being the focus of my current studies, transportation science is a very interesting area that is related to many of the mathematical fields I am interested in. Improving public transport in cities for example, feels like a more direct way of achieving a positive impact than many other potential directions I am currently considering. I also want to keep the calls to identifying relevant problems and not only focusing on interesting conceptual models in mind, because this might be a potential issue for me in the future.

## 24. Community structure in social and biological networks. (2002)
Girvan, M. & Newman, M. E. J.

**10.03.2025:** The authors consider a common property of networks, namely community structure, which describes that groups of nodes have much more connections to nodes in their community than outside. 
They propose a new way of detecting community structure.
Unlike in hierarchical methods where community centers are detected, this method detects edges of communities by calculating the betweenness centrality of edges, iteratively removing the ones with the highest centrality.
They show that this method works very well on computer-generated networks and real-world networks with known community strucutre.
Then, they apply their method to a research network and a food web which detects plausible community structures.

This is a nice application of using centrality measures. In the end, the authors hope that more efficient algorithms can be created and I am interested what algorithms exist today and if they are still based on this concept.

## 25.  Multi-Valued Model for Generating Complex Chaos and Fractals. (2024).
Zhang, Y., Hua, Z., Bao, H. & Huang, H.

**11.03.2025:** A simple method for generating chaotic 1D complex-valued maps is presented. 
The equation is given by $$z(j+1) = p_1 (z(j)^n)^{1/m} + p_2$$. 
As the function $$(\cdot)^{1/m}$$ is multi-valued, multiple outputs are generated at each timestep and only the principle value will be used to calculate the next step.
For a couple of smaller value combinations of $$m$$ and $$n$$ fixed points, their stability, sufficient conditions for chaotic behavior and exact values of Lyapunov exponents are calculated.
Then, bifurcation diagrams and attractors are plotted for various parameters and various metrics shown that indicate highly chaotic trajectories.
It is shown that these maps allow the creation of random number sequences and show that their method has many advantages over previous chaos-based random number generators such as theoretical tractability, computational efficiency and large chaotic range.

I am still searching for a way to combine my complex analysis background with nonlinear dynamics and while this paper did not entirely do that, it showed how this knowledge might be useful in this area and contains some references to further reading.
Additionally, some very nice looking fractals are in this paper, that I might recreate in the future.

## 26.  Maps of random walks on complex networks reveal community structure. (2008)
Rosvall, M. & Bergstrom, C. T.

**12.03.2025:** Simplifying complex networks creates a trade-off between omitting details and keeping important information.
The amount of information needed to describe a random walk on the network can be reduced by using a 2-scale structure: describing which community the walker is in and then what node the walker occupies in that community.
The authors suggest defining communities such that the information needed to describe random walks on the network is minimized and develop an algorithm that approximatly minimizes this.
The method is compared to a modularity approach, where communities are chosen such as to maximize the inter-community weights and minimize intra-community weights and it is argued that this represents two different ways of understanding networks: the authors approach views the essence of a network as its flows, while the modularity approach views it as the topological properties of the links.
Lastly, community structure of cross-journal citations is visualized revealing some interesting insights on the state of science at their time.

Obviously, it would be cool to see a current map of community structure in science based on the same aproach to see what has changed. 
The implementation details were outsourced to the supplementary material so I don't really know what they did.
I really liked this paper because it communicated their insights really well.

## 27.  Finding knowledge paths among scientific disciplines. (2014)
Yan, E.

**13.03.2025:** Citation counts between different scientific fields based on the subject classification of the Journal Citation Reports are analysed to analyse the knowledge flow among fields.
Directed shortest paths between disciplines were created where the edges are weighted based on the number of citations from one discipline to another. 
This is used to study how much disciplines cite each other and construct maps of knowledge flow between fields. For example, it is found that economics does not cite other fields very much and that knowledge from physics-, chemistry- and biomedicince-related fields can be accessed more easily than other fields.

I think that the way knowledge flow is studied here might have some methodological issues that muddy the strength of the results. I do like the knowledge maps though and they show mostly intuitive results.

## 28. Death and revival of chaos. (2016)
Kaszás, B., Feudel, U. & Tél, T. 

**14.03.2025:** The effects on chaotic behaviour under varying parameters is studied in this paper.
Snapshot attractors of a driven pendulum with exponentially decaying driving are shown and it is found that chaotic behaviour exists even when the driving force is very low, i.e. for parameter values where no chaos exists in the frozen system.
While no chaos exists, the dynamics is qualitatively similar to chaotic saddles existing for larger forcings.
The variability of trajectories over time is measured using the standard deviation of the angular velocities at snapshots and depending on the time-scale switching-off of the foring compared to the dissipative time-scale of the system, the speed at which variability decreases behaves differently.
The switching-on process is also briefly discussed, showing that chaoti behavior now takes longer to develop.

I think that this paper has some very interesting insights into the dynamics of non-autonomous systems but for my own future research I think that I would like to approach things a bit more mathematically, rather than the very qualitative view taken here because that, while potentially being more difficult, would likely give more concrete results.



# Papers

1. Aguirre, L. A. & Letellier, C. Modeling Nonlinear Dynamics and Chaos: A Review. Mathematical Problems in Engineering 2009, 238960 (2009). **35 pages**
2. Wilting, J. & Priesemann, V. 25 years of criticality in neuroscience — established results, open controversies, novel concepts. Current Opinion in Neurobiology 58, 105–111 (2019). **8 pages**
3. Terhaar, J., Vogt, L. & Foukal, N. P. Atlantic overturning inferred from air-sea heat fluxes indicates no decline since the 1960s. Nat Commun 16, 222 (2025). **17 pages**
4. Gross, T. & Blasius, B. Adaptive coevolutionary networks: a review. J. R. Soc. Interface. 5, 259–271 (2008). **13 pages**
5. Barzel, B. & Barabási, A.-L. Universality in network dynamics. _Nature Phys_ **9**, 673–681 (2013).**10 pages**
6. Alkhayuon, H. M. & Ashwin, P. Rate-induced tipping from periodic attractors: Partial tipping and connecting orbits. Chaos: An Interdisciplinary Journal of Nonlinear Science 28, 033608 (2018). **12 pages**
7. Irwin, E. G., Jayaprakash, C. & Munroe, D. K. Towards a comprehensive framework for modeling urban spatial dynamics. Landscape Ecol 24, 1223–1236 (2009). **14 pages**
8. Wilting, J. & Priesemann, V. Inferring collective dynamical states from widely unobserved systems. _Nat Commun_ **9**, 2325 (2018). **7 pages**
9. Krönke, J. _et al._ Dynamics of tipping cascades on complex networks. _Phys. Rev. E_ **101**, 042311 (2020). **9 pages**
10. Alkhayuon, H., Tyson, R. C. & Wieczorek, S. Phase tipping: how cyclic ecosystems respond to contemporary climate. Proceedings of the Royal Society A: Mathematical, Physical and Engineering Sciences 477, 20210059 (2021). **26 pages**
11. DeAngelis, D. L. & Diaz, S. G. Decision-Making in Agent-Based Modeling: A Current Review and Future Prospectus. _Front. Ecol. Evol._ **6**, (2019). **15 pages**
12. Battiston, F. _et al._ The physics of higher-order interactions in complex systems. _Nat. Phys._ **17**, 1093–1098 (2021) **6 pages**
13. Mangiarotti, S. & Huc, M. Can the original equations of a dynamical system be retrieved from observational time series? _Chaos: An Interdisciplinary Journal of Nonlinear Science_ **29**, 023133 (2019). **14 pages**
14. Feudel, U. _et al._ Homoclinic bifurcation in a Hodgkin–Huxley model of thermally sensitive neurons. _Chaos: An Interdisciplinary Journal of Nonlinear Science_ **10**, 231–239 (2000).**9 pages**
15. Grebogi, C., Ott, E. & Yorke, J. A. Metamorphoses of Basin Boundaries in Nonlinear Dynamical Systems. _Phys. Rev. Lett._ **56**, 1011–1014 (1986). **6 pages**
16. An, L. _et al._ Challenges, tasks, and opportunities in modeling agent-based complex systems. _Ecological Modelling_ **457**, 109685 (2021). **17 pages**
17. Kuhlbrodt, T. & Feudel, Homoclinic bifurcation in an ocean circulation box model **26 pages**
27. Milo, R. _et al._ Network Motifs: Simple Building Blocks of Complex Networks. _Science_ **298**, 824–827 (2002). **5 pages**
19. Ashwin, P., Wieczorek, S., Vitolo, R. & Cox, P. Tipping points in open systems: bifurcation, noise-induced and rate-dependent examples in the climate system. _Philos Trans A Math Phys Eng Sci_ **370**, 1166–1184 (2012). **22 pages**
20. Meisel, C. & Gross, T. Adaptive self-organization in a realistic neural network model. _Phys. Rev. E_ **80**, 061917 (2009). **7 pages**
21. Baer, S. M., Erneux, T. & Rinzel, J. The Slow Passage through a Hopf Bifurcation: Delay, Memory Effects, and Resonance. _ResearchGate_ (1989) doi:[10.1137/0149003](https://doi.org/10.1137/0149003).**18 pages**
22. Einstein, A. Über die von der molekularkinetischen Theorie der Wärme geforderte Bewegung von in ruhenden Flüssigkeiten suspendierten Teilchen. _Annalen der Physik_ **322**, 549–560 (1905). **12 pages**
23. Agatz, N., Hewitt, M. & Thomas, B. W. “Make no little plans”: Impactful research to solve the next generation of transportation problems. Networks 77, 269–286 (2021). **18 pages**
24. Girvan, M. & Newman, M. E. J. Community structure in social and biological networks. _Proc. Natl. Acad. Sci. U.S.A._ **99**, 7821–7826 (2002). **6 pages**
25. Zhang, Y., Hua, Z., Bao, H. & Huang, H. Multi-Valued Model for Generating Complex Chaos and Fractals. IEEE Transactions on Circuits and Systems I: Regular Papers 71, 2783–2796 (2024). **14 pages**
26. Rosvall, M. & Bergstrom, C. T. Maps of random walks on complex networks reveal community structure. Proceedings of the National Academy of Sciences 105, 1118–1123 (2008).
27. Yan, E. Finding knowledge paths among scientific disciplines. Journal of the Association for Information Science and Technology 65, 2331–2347 (2014). **17 pages**
28. Kaszás, B., Feudel, U. & Tél, T. Death and revival of chaos. _Phys. Rev. E_ **94**, 062221 (2016). **10 pages**

**Unread**

18. Review of Mathematical Modelling Techniques with Applications in Biosciences. ijcsm 135–144 (2022) doi:10.52866/ijcsm.2022.01.01.015. **10 pages**
19. Yan, E. Finding knowledge paths among scientific disciplines. Journal of the Association for Information Science and Technology 65, 2331–2347 (2014). **17 pages**

21. Schneider, T. D. Information Theory Primer. [https://www.fon.hum.uva.nl/rob/Courses/InformationInSpeech/CDROM/Literature/LOTwinterschool2006/www.lecb.ncifcrf.gov/~toms/paper/primer/primer.pdf](https://www.fon.hum.uva.nl/rob/Courses/InformationInSpeech/CDROM/Literature/LOTwinterschool2006/www.lecb.ncifcrf.gov/~toms/paper/primer/primer.pdf) (2005).**14 pages**
22. Perkins, T. J., Foxall, E., Glass, L. & Edwards, R. A scaling law for random walks on networks. _Nat Commun_ **5**, 5121 (2014). **7 pages**
23. Jones, J. Characteristics of pattern formation and evolution in approximations of physarum transport networks. _Artificial Life_ **16**, (2010). **28 pages**
10. Lorenz, E. N. Deterministic Nonperiodic Flow. _Journal of the Atmospheric Sciences_ **20**, 130–141 (1963).
11. Tipping elements in the Earth’s climate system. [https://www.pnas.org/doi/10.1073/pnas.0705414105](https://www.pnas.org/doi/10.1073/pnas.0705414105) doi:[10.1073/pnas.0705414105](https://doi.org/10.1073/pnas.0705414105). **8 pages**
12. Baker, J. A. _et al._ Continued Atlantic overturning circulation even under climate extremes. _Nature_ **638**, 987–994 (2025). **21 pages**

