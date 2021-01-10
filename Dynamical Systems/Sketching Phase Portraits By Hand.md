To draw a phase portrait by pen and paper, it is often instructive to first determine the [[Nullclines|nullclines]]


### Linear Example

$\dot x = 5x+y$
$\dot y = -x-y$

Nullclines
$\dot x=0\implies y=-5x$
$\dot y = 0\implies y=-x$

![[Nullclines Phase Portrait Linear Example.png]]

From the plotted [[Trajectory|trajectories]] we see that the [[Fixed Points|fixed point]] at the intersection of the [[Nullclines|nullclines]] is a saddle point. 

Consistency check

$\mathbb A=\begin{pmatrix}5&1\\-1&-1\end{pmatrix}\implies \Delta = \det \mathbb A=-4\implies$ Saddle point

### Non-Linear Example

$\dot x = x(3-2x-y)$
$\dot y = y(2-x-y)$

[[Nullclines]]

$\dot x = 0\implies x=0\vee x=(3-y)/2$
$\dot y=0\implies y=0\vee y=2-x$

We can analyze the [[Flow|flow]] on the [[Nullclines|nullclines]] as follows

|$\text{Nullcline}$|$x=0$|$x=(3-y)/2$|$y=0$|$y=2-x$|
|---|---|---|---|
|$\text{Flow}$|$\dot y = y(1-y)/2$|$\dot x=x(3-2x)$|$\dot x =x(1-x)$|

Which allows us to sketch the following [[Phase Portrait|phase portrait]]:

![[Nonlinear Phase Portrait Nullclines.png]]

The system has 4 [[Fixed Points|fixed points]] at the intersections of the two types of [[Nullclines|nullclines]] 
$(x_1^*,y_1^*)=(0,0)$, 
$(x_2^*,y_2^*)=(0,2)$, 
$(x_3^*,y_3^*)=(\frac 32,0)$, 
$(x_4^*,y_4^*)=(1,1)$.

The [[Nullclines|nullclines]] give a rough picture of the flow, but it can sometimes be hard to figure out what happens close to the fixed points using [[Nullclines|nullclines]] only. Therefore, use [[2D Linear Stability Analysis|linear stability analysis]] around the fixed points. 

In this case we have $\mathbb J = \begin{bmatrix}3-4x-y&-x\\-y&2-x-2y\end{bmatrix}$

This gives us the following table

|$\text{Fixed point }(x^*,y^*)$|$(0,0)$|$(0,2)$|$(3/2,0)$|$(1,1)$|
|----|----|----|----|----|
|$\tau\equiv\text{tr}\;\mathbb J(x^*,y^*)$|$5$|$-1$|$-5/2$|$-3$|
|$\Delta=\det\mathbb J(x^*,y^*)$|$6$|$-2$|$-3/2$|$1$|
|$\lambda_{1,2}=(\tau\pm \sqrt{\tau^2-4\Delta})/2$|$(2,3)$|$(-2,1)$|$(-3,1/2)$|$(-3\pm \sqrt 5)/2$|
|Type|[[Unstable Node]]|[[Saddle Point]]|[[Saddle Point]]|[[Stable Node]]|
|$\mathbf v_1$|$(0,1)$|$(0,1)$|$(1,0)$|$(1-\sqrt 5,2)$|
|$\mathbf v_2$|$(1,0)$|$(-3,2)$|$(-3/7,1)$|$(1+\sqrt 5,2)$|

For further analysis of this system, see the time reversible example at [[Sketching Phase Portraits By Hand]]

### [[Reversible Systems|Reversible System]] Example

Consider the system introduced in [[Reversible Systems]].

To sketch the full phase portrait, start with the [[Nullclines|nullclines]] and linearized dynamics around the saddle points  (evaluate the direction of the stable and unstable manifolds of the saddle points).

![[Reversible System Nullclines.png|500x400]]

The unstable trajectory going up from the lower saddle point must continue upwards ($\dot y >0$) until $y=0$ is reached with vertical slope ($\dot x = 0$ at $y=0$). 
Due to reversibility there must be a mirrored trajectory coming from the upper sadlle. The combined [[Heteroclinic Trajectory]] joins two fixed points.
Likewise, the unstable trajectory down from the upper saddle point must move down and meet  the $y=0$ line at some $x>0$.

At the crossing point it joins with its mirror from the lower saddle point, forming a second [[Heteroclinic Trajectory|heteroclinic trajectory]]. The heteroclinic trajectories form a [[Heteroclinic Cycle|heteroclinic cycle]] surrounding a region of closed orbits.  
