When is it safe to neglect the quadratic terms in the [[Linear Stability Analysis|stability analysis]]?

[[Linear Stability Analysis|Linear stability analysis]] gives a qualitatively correct picture if the fixed point is a [[Node]], [[Spiral]], or [[Saddle Point|Saddle]].

For the border-line cases [[Degenerate Node]], [[Star]], [[Center]], or [[Non-Isolated Fixed Point]] non-linear terms may (or may not) change the dynamics qualitatively from the border-line case to one of the neighbouring cases in the [[Delta Tau Diagram]]. 

To find what type the [[Fixed Points|fixed point]] is, one must analyze the non-linear dynamics close to the fixed point, either analytically, or using a [[Geometrical Approach|geometric approach]]

The non-linear terms change the type and stability of the fixed point in some cases (such as the example below). Similarly [[Star|stars]] and [[Degenerate Node|degenerate nodes]] can be changed into [[Spiral|spirals]] or [[Node|nodes]] by small non-linearities, but their stability does not change. 

More generally:
* If both $\text{Re}\;\lambda_1$ and $\text{Re}\;\lambda_2$ are non-zero ([[Stable Fixed Points|Attractors]], [[Unstable Fixed Points|Repellers]], [[Saddle Point|Saddle Points]]), the qualitative dynamics is robust to small perturbations. The fixed point is [[Hyperbolic|hyperbolic]] and the synamics is [[Structural Stability|structurally stable]]
* If $\text{Re}\;\lambda_1$ and/or $\text{Re}\;\lambda_2$ are zero ([[Center|Centers]] or [[Non-Isolated Fixed Point|Non-Isolated Fixed Points]]), the dynamics are [[Marginal Fixed Point|marginal]] and not [[Structural Stability|structurally stable]] 

### Non-Linear Analysis Example

Consider the system 
$\dot x =-y+ax(x^2+y^2)\equiv f(x,y)$
$\dot y = x+ay(x^2+y^2)\equiv g(x,y)$
We have one fixed point $(x^*,y^*)=(0,0)$ and [[Stability Matrix|stability matrix]].
$\mathbb J(x,y)=\begin{bmatrix}3ax^2+ay^2&-1+2axy\\1+2axy&ax^2+3ay^2\end{bmatrix}$
At the [[Fixed Points|fixed point]] $\mathbb J(0,0)=\begin{bmatrix}0&-1\\1&0\end{bmatrix}$.
with [[Eigenvalue|eigenvalues]] $\lambda_{1,2}=\pm i$. The [[Fixed Points|fixed point]] is a [[Center|center]] according to [[Linear Stability Analysis|linear stability analysis]].

Analyse the non-linear behaviour of the system. In [[Polar Coordinates|polar coordinates]] 
$r=\sqrt{x^2+y^2}$, $\theta=\text{atan}(y/x)$
$\implies \dot r = \frac{1}{2\sqrt{x^2+y^2}}(2x\dot x+2y\dot y)$
$=\frac{1}{r}(x[-y+ax(x^2+y^2)]+y[x+ay(x^2+y^2)])$
$=\frac{1}{r}(ax^2r^2+ay^2r^2)=ar^3$.

$\dot \theta=\left[\frac{d}{dx}\text{atan}(x)=\frac{1}{1+x^2}\right]=\frac{1}{1+(y/x)^2}\frac{d}{dt}\frac{y}{x}$
$=\frac{1}{1+(y/x)^2}\left(\frac{\dot y}{x}-\frac{y}{x^2}\dot x\right)=\frac{1}{x^2+y^2}(x\dot y-y\dot x)$
$=\frac{1}{r^2}(x[x+ay(x^2+y^2)]-y[-y+ax(x^2+y^2)])=\frac{1}{r^2}(x^2+y^2)=1$


The dynamics $\dot r = ar^3$ and $\dot \theta=1$ is simpler to analyze. If $a=0$ the system is linear and we have a [[Center|center]]. Otherwise, we have a spiral (unstable if $a>0$ or stable if $a<0$).

