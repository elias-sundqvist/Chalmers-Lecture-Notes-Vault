There is no general method to find conserved quantities in a given system, but here follows some useful cases methods for doing so:

#### Case 1
If the system can be written as 
$\ddot x =-V'(x)$ 
it has the conserved quantity 
$E=\frac{y^2}{2}+V(x)$
with 
$y=\dot x$.

#### Case 2
It is sometimes possible to search for an explicit relation between $y$ and $x$ by dividing $\dot y$ with $\dot x$. For example

$\dot x = y$
$\dot y = y^2-x$

gives
$\frac{\dot y}{\dot x}=\frac{dy}{dx}=\frac{y^2-x}{y}$
Let $\overset \sim y=e^{-x}y$ to get
$\frac{d\overset \sim y}{dx}=-e^{-x}y+e^{-x}\frac{dy}{dx}=-e^{-x}\frac{x}{y}=-e^{-2x}\frac{x}{\overset \sim y}$
solve by separation of variables
$\overset \sim yd\overset \sim y=-e^{-2x}xdx\implies \frac{\overset \sim y^2}{2}=\frac{1}{4}e^{-2x}(1+2x)+E$
with an integration constant $E$, which forms an [[Integral Of Motion|integral of motion]].

$E(x,y)=e^{-2x}\frac{y^2}{2}-\frac{1}{4}e^{-2x}(1+2x)$