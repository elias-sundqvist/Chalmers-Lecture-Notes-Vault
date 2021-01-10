---
alias:
  - Homoclinic Bifurcation
---
Consider a collision between a [[Limit Cycle|limit cycle]] and a [[Saddle Point|sadle point]] to form a [[Homoclinic Orbit|homoclinic orbit]].

$\dot x = y$
$\dot y = \mu y+ x-x^2+xy$

[[Global Bifurcations|Non-local bifurcation]] $\implies$ need to use computer! 

![[Numerical Bifurcation Of Homoclinic Orbit Illustration.png]]

For $\mu<\mu_{rmc}\approx -0.8645$ a [[Saddle Point|saddle point]] and a [[Limit Cycle|limit cycle]] are isolated (See [[Isolated Fixed Point]], [[Isolated Closed Orbits]])

as $\mu$ is increased, the [[Limit Cycle|limit cycle]] expands until it eventually collides with the [[Saddle Point|saddle point]] at $\mu=\mu_c$, forming a homoclinic orbit.

When $\mu>\mu_{rmc}$ the [[Homoclinic Orbit|homoclinic orbit]] breaks.

Note that the upper right unstable manifold lies inside of a [[Stable Manifold]] when $\mu<\mu_c$ and lies outside of the stable manifold when $\mu>\mu_c$. This property changes [[Topology Of Dynamical System|topology]] of the solution (see the purple trajectories), i.e. a [[Bifurcation|bifurcation]] occurs as $\mu$ passes $\mu_c$ also in a homoclinic bifurcation without collision with a limit cycle (the [[Homoclinic Orbit|homoclininc orbit]] instead surrounds a band of [[Closed Orbit|closed orbits]]). 

An example is a [[Josephson Junction]]. The homoclinic bifurcation is an example of an [[Infinite-Period Bifurcation]].