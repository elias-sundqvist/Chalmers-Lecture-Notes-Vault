---
alias:
  - Infinite Time Bifuraction
---
![[Infinite Period Bifurcation Illustration.png]]

An infinite period bifurcation that bifurcates by slowing an orbit down until it reaches an infinite [[Period Time]] 

One example of a infinite-period bifurcation is the [[Bifurcation Of Homoclinic Orbit|bifurcation of a homoclinic orbit]].

### Example
Consider the following system of uncoupled equations:

$\dot r=r(1-r^2)$
$\dot \theta=\mu-\sin \theta$

The $r$-equation is the typical equation for an [[Stable Limit Cycle|attracting limity cycle]] at $r=1$.

When $\mu>1$ we have a [[Stable Limit Cycle|stable limit cycle]] with a bottleneck (slow velocity) at $\theta=\frac \pi 2$

When $\mu=1$ a [[Semi Stable Fixed Points|half stable fixed point]] appears at $(r,\theta)=(1,\pi/2)$ $\implies$ it takes an infinite time to pass $\theta=\frac \pi 2$ along the [[Homoclinic Orbit|homoclinic orbit]] (former [[Limit Cycle]]). At $\theta=\pi/2$ the flow must be vertical towards $r=1$.

When $\mu<1$ a [[Saddle-Node Bifurcation|saddle node pair]] is formed, joined by [[Heteroclinic Trajectory|heteroclinic trajectories]]


As shown in [[Slow Passage]] the dynamics is slow close to the [[Saddle-Node Bifurcation|saddle-node bifurcation]]. (The time scale along the limit cycles scales as $\frac 1 {\sqrt{|\mu-1|}}$ for both sides of the bifurcation, see [[Period Time Scaling]]).

Another infinite-time bifurcation (with another [[Period Time Scaling|scaling in period time]] $T\sim \ln \mu$) is the [[Bifurcation Of Homoclinic Orbit|bifurcation of a homoclinic orbit]].