See [[Hopf Bifurcation]]

If a small-amplitude [[Limit Cycle|limit cycle]] is formed to catch the [[Unstable|unstable]] [[Trajectory|trajectories]] after the bifurcation, the bifurcation is supercritical. 

### Example

$\dot r = r(\mu-r^2)$
$\dot \theta=\omega$

Radial equation is on the form of a [[Supercritical Pitchfork Bifurcation|supercritical pitchfork]].
![[Hopf Bifurcation As Radial Pitchfork Bifurcation Illustrated.png]]

When $\mu<0$ the radial equation has a stable fixed point at $r^*=0$ (a [[Stable Spiral|stable spiral]] in $x,y$-space)
When $\mu>0$ the origin becomes an [[Unstable Spiral|unstable spiral]], but trajectories are caught at $r^*=\sqrt \mu$, i.e. [[Limit Cycle|limit cycle]] of radius $\sqrt \mu$ $\implies$ stable small-amplitude oscillations.


To verify that the eigenvalues cross $\text{Re}[\lambda_i]=0$ with nonzero $\text{Im}[\lambda_i]$ we need to convert to [[Cartesian Coordinates|cartesian corrdinates]] $x=r\cos \theta$, $y=r\sin \theta$.
Some algebra gives 

$\dot x = \mu x - \omega y +\text{cubic terms}$
$\dot y =\omega x + \mu y + \text{cubic terms}$

So the [[Stability Matrix|stability matrix]] of the [[Fixed Points|fixed point]] at the origin is 

$\mathbb J = \begin{bmatrix}\mu&-\omega\\\omega&\mu\end{bmatrix}$

Eigenvalues $\lambda=\mu\pm i\omega\implies$ [[Fixed Points|fixed point]] becomes [[Unstable|unstable]] for positive $\mu$.