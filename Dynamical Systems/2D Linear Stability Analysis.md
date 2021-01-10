Doing [[Linear Stability Analysis]] in 2d works as follows:

A [[2D Flows|2d flow]] can be written as 
$\dot x = f(x,y)$
$\dot y = g(x,y)$

and it has the fixed points $(x^*,y^*)$ where $f(x^*,y^*)=g(x^*,y^*)=0$.
By linearizing around the fixed point we get
$\eta = x-x^*$, $\mu=y-y^*$

$\frac{d}{dt}\begin{bmatrix}\eta\\\mu\end{bmatrix}=\mathbb J(x^*,y^*)\begin{bmatrix}\eta\\\mu\end{bmatrix}+\dots$, with $J(x^*,y^*)=\begin{bmatrix}\frac{\partial f}{\partial x}&\frac{\partial f}{\partial y}\\\frac{\partial g}{\partial x}&\frac{\partial g}{\partial y}\end{bmatrix}$

Where $\mathbb J$ is the [[Stability Matrix]] (a.k.a [[Stability Matrix|Jacobian Matrix]]) and the derivatives are evaluated at the fixed point $(x^*,y^*)$.

In linear stability analysis, the higher-order terms are neglected, and the deviation $\begin{bmatrix}\eta\\\mu\end{bmatrix}$ can be classified as in [[Classification Of Linear Flows|the case of linear flows]]