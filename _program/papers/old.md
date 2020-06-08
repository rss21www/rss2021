---
layout: paper
title: "Planning and Execution using Inaccurate Models with Provable Guarantees"
comments: true
invisible: true
---

*[Anirudh Vemula](https://vvanirudh.github.io/), [Yash Oza](https://www.ri.cmu.edu/ri-people/yash-oza/), [J. Andrew Bagnell](http://robotwhisperer.org/), [Maxim Likhachev](http://www.cs.cmu.edu/~maxim/index.html)*
{: style="color:gray; font-size: 120%; text-align: center;"}

### Abstract

Models used in modern planning problems to simulate outcomes of real world action executions are becoming increasingly complex, ranging from simulators that do physics-based reasoning to precomputed analytical motion primitives. However, robots operating in the real world often face situations not modeled by these models before execution. This imperfect modeling can lead to highly suboptimal or even incomplete behavior during execution. In this paper, we propose CMAX an approach for interleaving planning and execution. CMAX adapts its planning strategy online during real-world execution to account for any discrepancies in dynamics during planning, without requiring updates to the dynamics of the model. This is achieved by biasing the planner away from transitions whose dynamics are discovered to be inaccurately modeled, thereby leading to robot behavior that tries to complete the task despite having an inaccurate model. We provide provable guarantees on the completeness and efficiency of the proposed planning and execution framework under specific assumptions on the model, for both small and large state spaces. Our approach CMAX is shown to be efficient empirically in simulated robotic tasks including 4D planar pushing, and in real robotic experiments using PR2 involving a 3D pick-and-place task where the mass of the object is incorrectly modeled, and a 7D arm planning task where one of the joints is not operational leading to discrepancy in dynamics
{: style="color:gray; font-size: 120%; text-align: justified;"}



webpage: https://vvanirudh.github.io/blog/cmax/

video: https://youtu.be/eQmAeWIhjO8


<iframe width="560" height="315" src="https://www.youtube.com/embed/eQmAeWIhjO8" frameborder="0" allow=" encrypted-media" allowfullscreen></iframe>




{% comment %}
{% include disqus.html %}
{% endcomment %}