Consider a general [[Continuous Dynamical Systems|continuous dynamical system]] of dimensionality 2. 
$\dot{\mathbf x}=\mathbf f$ 
with $\mathbf x=(x_1,x_2)$ and $\mathbf g(\mathbf x)=(f_1(\mathbf x), f_2(\mathbf x))$. To have a clearer notation without indices, we often define. 

$x=x_1$, $y=x_2$, $f=f_1$, $g=f_2$, $\implies \cases{\dot x = f(x,y)\\\dot y = g(x,y)}$


The [[Trajectory|trajectory]] $\mathbf x(t)$ depends on the [[Initial Condition|initial condition]] $\mathbf x(0)$:

![[Trajectory With Initial Condition Illustrated.png]]

In [[Non-linear dynamical systems|non-linear systems]] it is usually not possible to find $\mathbf x(t)$ analytically. Phase portraits are typically much more complicated compared to the linear flows considered so far.  For example:

![[Complicated Non-Linear Phase Portrait Illustration.png]]

In the image above we have
* 3 [[Fixed Points|fixed points]] (A, B, C) ,  $\mathbf f(\mathbf x^*)=0$
	* (A, C) are [[Saddle Point|saddle points]]
	* (B) is a [[Spiral|spiral]]   ([[Unstable Spiral]]) 
	* (A,B,C) are [[Unstable|unstable]]
	* (D) is [[Stable|stable]]
* 1 [[Closed Orbit|Closed orbit]] (D), $[\text{Periodic solution }\mathbf x(t)=\mathbf x(t+T)]$


As for the [[Flows On The Line|one dimensional case]]: If the flow is smooth (both $\mathbf f$ and its partial derivatives $\partial_i f_j$ are continuous) is some open connected domain $D\in \mathbb R^n$, then for $\mathbb x_0\in D$ the [[Initial Value Problem|initial value problem]] has a unique solution in some time interval around $t=0$

As a consequence [[Trajectory|trajectories]] *cannot intersect*. IF they did, there would be two solutions starting from the point of intersection, which would break the uniqueness condition. 