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
- Break Time (vacation): 12th - 23rd of February
- End Date: 18th of March

Total: 30 Days

**Paper selection:** First, some survey papers from different fields were selected. 
Additionally, some papers related to potential master's thesis topics were included.
Lastly, some papers that just sounded interesting or were written by some of my professors were selected as well.
In total, 15 papers were selected in order to leave room open for follow up research.
In the unlikely case that anyone reads this before I am finished, any paper suggestions are welcome as well (send me an email to ole.schuegl@uni-oldenburg.de).

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

# Papers
(Not in order)

1. Aguirre, L. A. & Letellier, C. Modeling Nonlinear Dynamics and Chaos: A Review. Mathematical Problems in Engineering 2009, 238960 (2009). **35 pages**
2. Wilting, J. & Priesemann, V. 25 years of criticality in neuroscience — established results, open controversies, novel concepts. Current Opinion in Neurobiology 58, 105–111 (2019). **8 pages**
3. Terhaar, J., Vogt, L. & Foukal, N. P. Atlantic overturning inferred from air-sea heat fluxes indicates no decline since the 1960s. Nat Commun 16, 222 (2025). **17 pages**
4. Gross, T. & Blasius, B. Adaptive coevolutionary networks: a review. J. R. Soc. Interface. 5, 259–271 (2008). **13 pages**
5. Barzel, B. & Barabási, A.-L. Universality in network dynamics. _Nature Phys_ **9**, 673–681 (2013).**10 pages**
6. Alkhayuon, H. M. & Ashwin, P. Rate-induced tipping from periodic attractors: Partial tipping and connecting orbits. Chaos: An Interdisciplinary Journal of Nonlinear Science 28, 033608 (2018). **12 pages**
7. Irwin, E. G., Jayaprakash, C. & Munroe, D. K. Towards a comprehensive framework for modeling urban spatial dynamics. Landscape Ecol 24, 1223–1236 (2009). **14 pages**
8. Wilting, J. & Priesemann, V. Inferring collective dynamical states from widely unobserved systems. _Nat Commun_ **9**, 2325 (2018). **7 pages**
9. Krönke, J. _et al._ Dynamics of tipping cascades on complex networks. _Phys. Rev. E_ **101**, 042311 (2020). **9 pages**

10. Agatz, N., Hewitt, M. & Thomas, B. W. “Make no little plans”: Impactful research to solve the next generation of transportation problems. Networks 77, 269–286 (2021). **18 pages**
11. Review of Mathematical Modelling Techniques with Applications in Biosciences. ijcsm 135–144 (2022) doi:10.52866/ijcsm.2022.01.01.015. **10 pages**
12. Alkhayuon, H., Tyson, R. C. & Wieczorek, S. Phase tipping: how cyclic ecosystems respond to contemporary climate. Proceedings of the Royal Society A: Mathematical, Physical and Engineering Sciences 477, 20210059 (2021). **26 pages**
13. Yan, E. Finding knowledge paths among scientific disciplines. Journal of the Association for Information Science and Technology 65, 2331–2347 (2014). **17 pages**
14. Zhang, Y., Hua, Z., Bao, H. & Huang, H. Multi-Valued Model for Generating Complex Chaos and Fractals. IEEE Transactions on Circuits and Systems I: Regular Papers 71, 2783–2796 (2024). **14 pages**
15. DeAngelis, D. L. & Diaz, S. G. Decision-Making in Agent-Based Modeling: A Current Review and Future Prospectus. _Front. Ecol. Evol._ **6**, (2019). **15 pages**
16. Schneider, T. D. Information Theory Primer. [https://www.fon.hum.uva.nl/rob/Courses/InformationInSpeech/CDROM/Literature/LOTwinterschool2006/www.lecb.ncifcrf.gov/~toms/paper/primer/primer.pdf](https://www.fon.hum.uva.nl/rob/Courses/InformationInSpeech/CDROM/Literature/LOTwinterschool2006/www.lecb.ncifcrf.gov/~toms/paper/primer/primer.pdf) (2005).**14 pages**
17. Perkins, T. J., Foxall, E., Glass, L. & Edwards, R. A scaling law for random walks on networks. _Nat Commun_ **5**, 5121 (2014). **7 pages**
18. An, L. _et al._ Challenges, tasks, and opportunities in modeling agent-based complex systems. _Ecological Modelling_ **457**, 109685 (2021). **17 pages**
19. Battiston, F. _et al._ The physics of higher-order interactions in complex systems. _Nat. Phys._ **17**, 1093–1098 (2021) **6 pages**
20. Feudel, U. _et al._ Homoclinic bifurcation in a Hodgkin–Huxley model of thermally sensitive neurons. _Chaos: An Interdisciplinary Journal of Nonlinear Science_ **10**, 231–239 (2000).**9 pages**
21. Jones, J. Characteristics of pattern formation and evolution in approximations of physarum transport networks. _Artificial Life_ **16**, (2010). **28 pages**
22. Mangiarotti, S. & Huc, M. Can the original equations of a dynamical system be retrieved from observational time series? _Chaos: An Interdisciplinary Journal of Nonlinear Science_ **29**, 023133 (2019). **14 pages**
23. Grebogi, C., Ott, E. & Yorke, J. A. Metamorphoses of Basin Boundaries in Nonlinear Dynamical Systems. _Phys. Rev. Lett._ **56**, 1011–1014 (1986). **6 pages**
24. Kuhlbrodt, T. & Feudel, Homoclinic bifurcation in an ocean circulation box model **26 pages**