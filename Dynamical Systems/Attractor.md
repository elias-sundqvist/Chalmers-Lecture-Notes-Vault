An attractor is defined as 

1. An invariant set: [[Trajectory|trajectories]] starting on the attractor can not leave it.
2. Attracting: There exists an open set of initial conditions that contains the attractor and whose [[Trajectory|trajectories]] reach the attractor as $t\rightarrow \inf t$. The [[Stable Manifold|Basin Of Attraction]] is the largest such set.  (If this condition is not fulfilled we have a [[Limit Set]])
3. Minimal: No subset on the attractor satisfies conditions $1$ and $2$. 

Examples of attractors are [[Fixed Points|fixed points]] and [[Limit Cycle|limit cycles]].

### Practice Examples

#### 1. [[Heteroclinic Trajectory]] $\Gamma_1$ Between A [[Saddle Point|Saddle]] And [[Stable Node]]
![[Heteroclinic Trajectory Between Saddle And Stable Node Illustration.png]]

A [[Heteroclinic Trajectory|heteroclinic trajectory]] between (and including) a [[Saddle Point|saddle]] and a [[Stable Node|stable node]], $\Gamma_1$, satisfies condition 1 ([[Trajectory|trajectories]] starting on $\Gamma_1$ remain on $\Gamma_1$) and $\Gamma_1$ is attractive, but it is not minimal - there is a subset (the [[Node|node]]) that satisfies 1 and 2. $\implies$ the node is the attractor. 

#### 2. [[Heteroclinic Cycle]] Between Two [[Saddle Point|Saddle Points]]

![[Heteroclinic Cycle Between Two Saddle Points Illustration.png]]

A [[Heteroclinic Cycle|heteroclinic cycle]] between two [[Saddle Point|saddle points]], $\Gamma_2$ surrounding an unstable spiral. The candidate invariant sets are $\Gamma_2$ or the two saddles. Which saddle a trajectory starting inside the cycle ends up at as $t\rightarrow \infty$ can not be determined (for any large $t$ we can make $t$ even larger in order to closely follow a [[Heteroclinic Trajectory|heteroclinic trajectory]] to the opposite [[Saddle Point|saddle]]). THis implies that both [[Saddle Point|saddles]] and the interconnecting heteroclinic trajectories would constitute the minimal invariant set. However, since the region outside of the cycle is not attracted, we cannot create an [[Open Set|open set]]  of initial conditions containing $\Gamma_2$ and the saddle points. The cycle is therefore not an attractor, it is instead a [[Limit Set|limit set]] of the [[Trajectory|trajectories]] inside the [[Heteroclinic Cycle|cycle]].

