### 1D Saddle-Node Bifurcation

Consider a general system $f(x,r)$ with constant parameter $r$ changing smoothly for different values of $r$ as illustrated below:
![[Saddle-Node Bifurcation Illustration.png]]
* If $r<r_c$: 4 fixed points. The system ends up at one of the two [[Stable]] ones (or run away to infinity). The dynamics do not change qualitatively as $r$ changes. 
* When $r=r_c$ the maximum happens to pass the $\dot x=0$ axis ([[Marginal Fixed Point]])
* When $r>r_c$ there is a qualitative change in the dynamics: two fixed points have merged and dissapeared and all trajectories end up and the remaining [[Stable Fixed Points|stable fixed point]].

### 2D Saddle-Node Bifurcation

Assume that a [[Saddle Point|saddle point]] and an [[Stable Node|attracting node]] collide as a parameter $\mu$ is varied.

This happens when [[Fixed Points|fixed points]] are formed at intersections of [[Nullclines|nullclines]]. As $\mu$ is varied, the [[Nullclines|nullclines]] deform continuosly. If they slip through each other the fixed points collide. 

![[Saddle Node Nullcline Collision Illustration.png]]

Change coordinates to the local [[Eigenframe|eigenframe]] of the [[Saddle Point|saddle point]]. Let the unstable directions of the [[Saddle Point|saddle]] be $\hat{\mathbf v}_u=\pm(1,0)$ and the stable directions $\hat{\mathbf v}_u=\pm(0,1)$When the [[Node|node]] comes closeby, it must merge along the [[Unstable Manifold|unstable manifold]] of the [[Saddle Point|saddle]] (otherwise trajectories could not remain continuous and linear as the fixed points merge)

![[2D Saddle Node Bifurcation Illustration.png]]

The bifurcation is essentially one-dimensional (in any dimension). 
The normal form is

$\dot x = \mu+x^2$ (same as [[Normal Form Of Saddle-Node Bifurcation|1D]])
$\dot y = -y$

The vicinity of each of the two fixed points is characterized using the [[Stability Matrix|stability matrix]] evaluated at the fixed points. The two [[Eigenvalue|eigenvalues]] (one for each fixed point) corresponding to the direction of the interconnecting manifold have opposite signs $\implies$ at the bifurcation point (at least) one eigenvalue must vanish.

After bifurcation a slow region remains ([[Ghost Of Fixed Points]]) before the bifurcation $T_{\text{pass}}=\indty$ (along interconnecting manifold), after bifurcation $T_{\text{pass}}$ decreases smoothly: $T_{\text{pass}}\sim 1/\sqrt{\mu-\mu_c}$

If there is a [[Unstable Node|repelling node]] everything works as described above, but with the arrows reversed. 