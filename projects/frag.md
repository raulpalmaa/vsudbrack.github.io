---
layout: post
title: 'Population dynamics in highly fragmented landscapes'
---

Human action fragments the natural habitat of several species all around the world. Understanding the effects of fragmentation to ecosystems is key to elaborate the best policies to avoid species extinctions. Therefore, it is important to study how the populations and ecosystems respond to these kinds of changes in landscapes. Well, if you experienced the ecological debates from the 70s, these ideas might remind you of the question: **single large or several small ecological reserves?**. This simple question, abbreviated by *SLOSS*, has evolved for almost half a century and the answer is, up to this day, very arguable. We humourly refer to this heated discussion as **FragWars**.

{% include quote.html text="Theory without fact is phantasy; but fact without theory is chaos. Divorced, both are useless; united, they are equally essential and fruitful." author="Charles Otis Whitman" %}

Perhaps, one of the most important progresses of this question was to change it from a binary point of view - i.e. *compact versus fragmented* -  to a continuous problem, **investigating the effect of the degree of fragmentation to the ecological value of landscapes**. It is also important to distinguish between fragmentation and the *fragmentation process*. This latter occurs simultaneously with habitat loss and, therefore, is always detrimental to ecosystems. To make this distinction even clearer, we refer to the difference of spatial configuration while keeping the total habitat amount constant as *fragmentation per se*. 

Since there are no two regions differing purely by **spatial configuration**, statistical techniques must be applied to observational data in order to isolate the effects of *fragmentation per se* on abundance, richness, evenness, or other **metrics of ecological value**. And this point is exactly where we believe that computational techniques may be a powerful tool to help researchers to **test hypotheses, mechanisms and concepts** and even **generate controlled artificial data** in order to analyse the suitability of statistical techniques. 

In 2020, I was invitedd to give a seminar about it on *EcoEncontros* at IB-USP. We can check the slides and the link for the video with the lecture below.

{% include image.html url="/assets/docs/projects/frag/FragWars.pdf" image="projects/frag/fragwars.png" text="Check the slides of this presentation" %}

In our project, we use numerical methods to simulate **Reaction-Diffusion Equations (FKPP Equations) in artificial landscapes** generated with different structural distributions while keeping the total amount of habitat constant. This guarantees we are observing phenomena caused by *fragmentation per se*. We discuss the net effects of fragmentation into the steady total population. In order to do that correctly, we established the correlation between fragmentation metrics with fixed amount of habitat, to ensure that conclusions are not biased by interdependencies of metrics (see a further discussion in the next section). 

We have also analytically calculated the critical size to allow population growth for bidimensional landscapes within our model, with given symmetries. These results prove that **habitat area is not the only factor** when it comes to population settling, and hence **patch shape matters**. 


In the future we will also explore consequences of fragmentation to communities. 

This work is done under **Roberto A. Kraenkel** supervision at IFT - UNESP and collaboration with **[Renato M. Coutinho](http://professor.ufabc.edu.br/~renato.coutinho/)** and financed by [FAPESP (Grant #2018/23984-0)](https://bv.fapesp.br/pt/bolsas/183763//).

There are a few subprojects available to undergraduate students, if **this discussion sounds appealing to you, get in touch :)**

## How to measure fragmentation? How to create a landscape?

We measure fragmentation in a continuous way through *fragmentation metrics*. There are many metrics, some measure different fragmentation aspects and a few are redundant, i.e. highly correlated to others in a context. Some examples are **complexity and entropy metrics**, such as Shannon Entropy and Mutual information; or metrics of **geometric features**, like Perimeter-Area fractal dimension, average Circumscribed Circle or simply, Perimeter-Area ratio. Others focus on average **patch shapes**, as their Mean Area or Edge density, while others yet focus on a **landscape-level**, as the number of patches, the % of habitat in the largest patch (LPI) or the average Euclidean distance between patches. 

Also, in order to study the effects of *fragmentation per se* in population dynamics numerically, we have to **simulate artificial landscapes**. There several different methods to generate them, and they are known as *Neutral Landscape Methods*. In the videos below, I show 2000 artificial landscapes, ordered from slightly fragmented to highly fragmented, for four methods. Firstly, I show the **Fractional Brownian Motion (FBM) method**, in which we ordered the landscapes by the *fractal dimension* (between 0 and 2), going from slightly to highly fragmented. 

{% include video.html src="https://www.youtube.com/embed/788kqrvQnyA" %}

The second, artificial **Mosaic Tessellation (MTS)** landscapes ordered by number of germs, centroid points for a Voronoy tessellation, going from slightly to highly fragmented. 

{% include video.html src="https://www.youtube.com/embed/oZXa7XT80Gk" %}

Below, we have artificial **Random Rectangular Clustering (RRC)** landscapes, descendingly ordered by average rectangle area (average of minimum and maximum length of suporposing rectangles), going from slightly to highly fragmented. 

{% include video.html src="https://www.youtube.com/embed/xgNKsu7eK5M" %}

Finally, artificial **Midpoint Displacement (MPD)** landscapes ordered by spatial correlation  (roughness), going from highly  compact to highly fragmented. 

{% include video.html src="https://www.youtube.com/embed/Vx_gpdr_AYc" %}

Can you se how **different methods impose different characteristics to landscapes** and their fragmentation metrics? It also change how this set of metrics is coupled, i.e. their correlations. It is a challenge to understand **how these characteristics reflect ecologically** under basic mechanisms. 

## How do patches communicate?

Recent explorations on our model revealed the presence of different movement scales, intra-patch and inter-patches. We are now working on how fragmentation affects features of population spatial distribution and investigating regimes of fragmentation that allow non-interactive (or weakly interacting) subpopulations to form - i.e. low interpatch communication. Forming networks of patches can help us understand further the *functional patches*, patches of "populations" rather than the geographical ones. 

## How does fragmentation affect the coexistance of species?

In the particular scenario of competition, how does fragmentation affect the coexistance of species? Could this model explain the interspecific competition release due to the presence of matrix mentioned in the literature? How the geographical fragmentation induces population clustering in two species?

This work is done with **[Cristóbal López](https://www.ifisc.uib-csic.es/en/people/cristobal-lopez/)** and **[Emilio Hernández-García](https://ifisc.uib-csic.es/users/emilio/)** at the *[Institute for Cross-Disciplinary Physics and Complex Systems (IFISC)](https://www.ifisc.uib-csic.es/en/)* of *[University of the Balearic Islands (UiB)](https://www.uib.eu/)* in Palma de Mallorca, Spain,  financed by [FAPESP (Grant #2019/02526-0)](https://bv.fapesp.br/pt/bolsas/190605/padroes-espaciais-na-distribuicao-populacional-em-paisagens-altamente-fragmentadas/).




