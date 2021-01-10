One mechanism that forms [[Closed Orbit|closed orbits]] is invariance under the simultaneous tranformation $t\rightarrow -t$ and $y\rightarrow -y$. 
This is called a reversible system.

This transformation mirrors [[Trajectory|trajectories]] in the upper half plane on the lower half plane. 

A special case of reversible systems are [[Time Reversible Systems]]

Reversible or [[Conservative Systems|conservative systems]] tend to have [[Trajectory|trajectories]] connecting one fixed point with itself ([[Homoclinic Orbit|homoclinic orbits]], see for example the [[Double-Well Potential]]) or with another fixed point ([[Heteroclinic Trajectory|heteroclinic trajectory]]).

### Example

Consider the system

$\dot x = y-y^3$
$\dot y = -x-y^2$

The system has three fixed points
$(x_1^*,y_1^*)=(-1,-1)$
$(x_2^*,y_2^*)=(0,0)$
$(x_3^*,y_3^*)=(-1,1)$

Using [[2D Linear Stability Analysis]], we get 

$\mathbb J =\begin{bmatrix}\frac{\partial f}{\partial x}&\frac{\partial f}{\partial y}\\\frac{\partial g}{\partial x}&\frac{\partial g}{\partial y}\end{bmatrix}=\begin{bmatrix}0&1-3y^2\\-1&-2y\end{bmatrix}$

which gives the following classification table


|[[Fixed Points]]|$(-1,-1)$|$(0,0)$|$(-1,1)$|
|----|----|----|----|
|[[Eigenvalue]]s|$1\pm \sqrt 3$|$\pm i$|$-1\pm \sqrt 3$|
|Type|[[Saddle Point]]|[[Center]]|[[Saddle Point]]|
|[[Stable Direction]]|$\frac{1}{\sqrt{5+2\sqrt 3}}\begin{bmatrix}1+\sqrt 3\\1\end{bmatrix}$|-|$\frac{1}{\sqrt{5-2\sqrt 3}}\begin{bmatrix}-1+\sqrt 3\\1\end{bmatrix}$|
|[[Unstable Direction]]|$\frac{1}{\sqrt{5-2\sqrt 3}}\begin{bmatrix}1-\sqrt 3\\1\end{bmatrix}$|-|$\frac{1}{\sqrt{5+2\sqrt 3}}\begin{bmatrix}-1-\sqrt 3\\1\end{bmatrix}$|

This shows that the origin is a [[Center|center]], but the nonlinear terms could destabilise, there is no [[Conservation Laws|conservation law]] as for the [[Conservative Systems|conservative systems]]. However, the system is [[Reversible Systems|reversible]]: invariant under the simultaneous transform $t\rightarrow -t$ and $y\rightarrow -y$.

Close to the origin, the center causes swirl for positive values of $y$. Time reversibility mirrors the solution in the line $y=0$ and trajectories must therefore close. This rules out spirals. 

![[Reversible System Closing Trajectories.png]]

For further analysis of this system, see [[Sketching Phase Portraits By Hand]]