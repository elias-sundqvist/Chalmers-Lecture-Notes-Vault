At the [[Bifurcation Point]] of a [[Saddle-Node Bifurcation]] (i.e. when $r=0$ in [[Normal Form Of Saddle-Node Bifurcation|the normal form]])

we simply get $\dot x = x^2$
$x^*=0$ is a [[Marginal Fixed Point]], so [[Linear Stability Analysis|linear stability analysis]] is not sufficient to analyze the stability of the fixed point. 

Using a [[Geometrical Approach|gaometric approach]] we can see that it is [[Semi Stable Fixed Points|semi stable]].

![[Semi Stable FP for Saddle-Node Bifurcation.png]]

We can get an exact solution through [[Separation of Variables|separation of variables]].

$\frac{1}{x^2}dx=dt$

Integrate from $t=0$ to $t$ ($x$ goes from $x(0)=x_0$ to $x(t)$)
$\frac{1}{x_0}-\frac{1}{x(t)}=t\implies x(t)=\frac{1}{\frac{1}{x_0}-t}=\frac{x_0}{1-x_0t}$

From this we can note the following things:
* Starting at $x_0>0$, it takes a finite time, $t=\frac{1}{x_0}$, to each $x=+\infty$
* When $t>\frac 1{x_0}$ the trajectory reappears from $x=-\infty$ and eventually approaches $x=0$ from the left.
* It takes infinite time to reach $x=0$.

The jump from $+\infty$ to $-\infty$ could not have been predicted by the [[Geometrical Approach|geometrical approach]] alone. Note, however, that we need to be careful in interpreting this result: depending on the physical system we want to model, the behaviour after $+\infty$ has been reached may be undefined.


