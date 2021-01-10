The [[Normal Form Of Bifurcations|normal form]] of a [[Saddle-Node Bifurcation|saddle-node bifuraction]] is $\dot x=r+x^2$. 
In 2D it is the same, with the addition of $\dot y=-y$.

When $1\gg r>0$ we have a [[Slow Passage|slow pasage]]
When $-1\ll r<0$ we have the [[Indications Of A Catastrophe|indications of a catastrophe]]
When $r=0$, see [[Saddle-Node Bifurcation Point Behaviour]]


Below follows the derivation:

Consider a general [[Flow|flow]] with parameter $r$, $\dot x(t)=f(x(t),r)$, with a [[Saddle-Node Bifurcation|saddle-node bifurcation]] at $x=x^*$ and $r=r_c$. For the [[Saddle-Node Bifurcation|saddle-node bifurcation]] to occur, $f(x,r)$ must have two close-by roots in $x$:
![[General Saddle-Node Bifurcation illustration.png]]

$f(x,r)$ always looks parabolic in $x$ close to the bifurcation (universal behavior).

At $r=r_c$, $x^*$ is a double root: $f(x^*,r_c)=\frac{\partial f}{\partial x}(x^*,r_c)=0$.
Expand $f$ around $x^*$ and $r_c$ to lowset contributing orders.

$f(x,r)=\underbrace{f(x^*,r_c)}_{=0}+\underbrace{\frac{\partial f}{\partial x}(x^*,r_c)}_{=0}(x-x^*)+\frac{\partial f}{\partial r}(x^*,r_c)(r-r_c)+\frac 12 \frac{\partial^2f}{\partial x^2}(x^*,r_c)(x-x^*)^2+\dots$.

Introduce rescaled coordinates $X=a(x-x^*)$ and $R=b(r-r_c)$.

$\dot X=a\dot x=\frac{a}{b}\frac{\partial f}{\partial r}(x^*,r_c)R+\frac{1}{2a}\frac{\partial^2 f}{\partial x^2}(x^*,r_c) X^2+\dots$.
Choose $a=\frac 12 \frac{\delta^2 f}{\delta x^2}(x^*,r_c),b=a\frac{\partial f}{\partial r}(x^*,r_c)$
$\dot X=R+X^2+\dots$.

In conclusion, a system has a [[Saddle-Node Bifurcation|saddle-node bifurcation]] if $f(x^*,r_c)=\frac{\partial f}{\partial x}(x^*,r_x)=0$ while $\frac{\partial^2f}{\partial x^2}(x^*,r_c)\ne 0$ and $\frac{\partial f}{\partial r}(x^*,r_c)\ne 0$. Close to the bifurcation point, the system can be written on the form $\dot x=r+x^2$.
