Consider the [[Van Der Pol Oscillator|van der Pol oscillator]] with $0<\mu\ll 1$ and some initial condition $x(0)=0$, $\dot x(0)=1$ (arbitrary condition that starts off the limit cycle).

### Solution using regular [[Perturbation Theory]]

Search for a solution for small values of $\mu$ by a series expansion.

$x(t)=x_0(t)+\mu x_1(t)+\mu^2x_2(t)+\dots$

insert this expansion into the [[Van Der Pol Oscillator|van der Pol oscillator]] equation and colect terms to order $\mu$.

$0=\ddot x+\mu(x^2-1)\dot x+x$
$=[\ddot x_0+\mu\ddot x_1]+\mu([x_0+\mu x_1]^2-1)[\dot x_0+\mu\dot x_1]+[x_0+\mu\dot x_1]+O(\mu^2)$
$=\ddot x_0+x_0+\mu[\ddot x_1+(x_0^2-1)\dot x_0+x_1]+O(\mu^2)$.

With initial conditions 

$0=x(0)=\underbrace{x_0(0)}_{=0}+\mu\underbrace{x_1(0)}_{=0}$
$1=\dot x(0)=\underbrace{\dot x_0(0)}_{=1}+\mu\underbrace{\dot x_1(0)}_{=0}$

To order $\mu^0$ we have 

$\ddot x_0+x_0=0\implies x_0(t)=\sin(t)$

To order $\mu^1$ we have

$\ddot x_1+(\sin^2 t-1)\cos t+x_1=0\implies x_1(t)=(6t+\sin(2t))(\sin t)/16$

Problem: $x_1$ contains [[Secular Terms|secular terms

thus the perturbation theory fails to describe the formation of the limit cycle (the amplitude of oscillations frow to infinity). Even though the perturbation theory is identical to the series expansion of the actual solution, it fails for times of order $t\sim \frac 1 \mu$.

![[Van Der Pol Oscillator With Small Mu Perturbation Theory Illustration.png]]

### Solution Using [[Two-Timing]]

In order to obtain a perturbation theory valid for large values of $t$, we need to make a higher-order expansion. Alternatively, we can notice that there are  (at least) two time scales in the problem: one for the oscillations (fast, $O(1)$), and one for the peak amplitude (slow, $O(1/\mu)$).
Separating these time scales in the perturbation expansion, so called [[Two-Timing|two-timing]], gives more accurate results for large $t$ even though we only consider the lowest order in $\mu$.

Evaluate the time derivatives

$\dot x = \frac{dx}{dt}=\underbrace{\frac{\partial x}{\partial \tau}}_{\partial_\tau x}\underbrace{\frac{d\tau}{dt}}_{1}+\underbrace{\frac{\partial x}{\partial T}}_{\partial_T x}\underbrace{\frac{dT}{dt}}_{\mu}=\partial_\tau x+\mu\partial_Tx$
$\ddot x = \partial_\tau\dot x+\mu\partial_T \dot x=\partial_\tau^2x+2\mu \partial_\tau\partial_T x+O(\mu^2)$

Make expansion in terms of small $\mu$, $x(\tau,T)=x_0(\tau,T)+\mu x_1(\tau+T)+\dots$, and insert this into the [[Van Der Pol Oscillator|van der Pol equation]].

$0=\ddot x+\mu(x^1-1)\dot x+x$
$=\partial_\tau^2x+2\mu \partial_\tau\partial_Tx+\mu(x^2-1)[\partial_\tau x+\mu\partial_Tx]+x+O(\mu^2)$
$=\partial_\tau^2x+x+\mu[2\partial_\tau\partial_Tx+(x^2-1)\partial_\tau x]+O(\mu^2)$
$=\partial_\tau^2[x_0+\mu x_1]+[x_0+\mu x_1]+\mu[2\partial_\tau\partial_Tx_0+([x_0]^2-1)\partial_\tau[x_0]]+O(\mu^2)$
$=\partial_\tau^2x_0+x_0+\mu[\partial_\tau^2x_1+x_2+2\partial_\tau\partial_Tx_0+([x_0]^2-1)\partial_\tau[x_0]]+O(\mu^2)$

To order $\mu^0$ we have
$\partial_\tau^2x_0+x_0=0\implies x_0=A(T)\sin\tau+B(T)\cos\tau$

where $A(T)$ and $B(T)$ are $T$-dependent coefficients. The initial condition for $x_0$

$0=x(0)=\underbrace{x_0(0,0)}_{=0}+\mu\underbrace{x_1(0,0)}_{=0}+\dots$
$1=\dot x(0)=\underbrace{\partial_\tau x_0(0,0)}_{=1}+\mu\underbrace{[\partial_Tx_0(0,0)+\partial_\tau x_1(0,0)]}_{=0}+\dots$

gives $A(T)$ and $B(T)$ as any functions satisfying $A(0)=1$, $B(0)=0$

To order $\mu^1$ we have

$0?\partial_\tau^2 x_1+x_1+2\partial_\tau\partial_T[A(T)\sin \tau+B(T)\cos\tau]+([A(T)\sin \tau+B(T)\cos\tau]^2-1)\partial_\tau[A(T)\sin \tau+B(T)\cos\tau]$
$=\partial_\tau^2x_1+x_1+2(A'(T)\cos\tau-B'(T)\sin \tau)+([A(T)+\sin \tau+B(T)\cos\tau]-1)[A(T)\cos\tau-B(T)\sin \tau]$

This equation can be solved for $x_1$  preferably using mathematica.  The solution contains a secular term on the form $f_1(T)\tau\sin\tau+f_2(T)\tau\cos\tau$
with 

$f_1(T)=-A'(T)+A(T)(4-A(T)^2-B(T)^2)/8$
$f_2(T)=-B'(T)+B(T)(4-A(T)^2-B(T)^2)/8$

We coose the functions A and B in a self-consistent manner as to remove the secular divergence from the terms proportional to $\tau\sin\tau$ and $\tau \cos\tau$, i.e. we solve $f_1=f_2=0$ for $A(T)$ and $B(T)$ with $A(0)=1$ and $B(0)=0$ (again, using Mathematica)

From this we get 

$A(T)=\frac{2}{\sqrt{1+3e^{-T}}}$, $B(T)=0$

IN conclusion, the [[Two-Timing|two-timing]] gives the solution 

$x(t)=A(T)\sin\tau=\frac{2}{\sqrt{1+3e^{-\mu t}}}\sin t$

To lowest order in $\mu$ the van der Pol oscillator approaches a circular limit cycle wth amplitude $\lim_{T\rightarrow \infty}A(T)=2$. The [[Two-Timing|two-timing]] result fro $x(t)$ agrees very well with the numerical solution, also for large times.

![[Van Der Pol Oscillator With Small Mu Two-Timing Perturbation Theory Illustration.png]]


### Solution By Averaging Over Fast Variable

If we are not interested in the fast dynamics, an easier method than two-timing, frequently applied in mechanics, is to average over the fast variable. Consider [[Van Der Pol Oscillator|van der Pol's equation]] as a dynamical system

$\dot x=y$
$\dot y=-x-\mu(x^2-1)y$
Change to polar coordinates

$r=\sqrt{x^2+y^2}$, $\phi=\text{arctan}(y/x)$

to obtain

$\dot r=\frac{x\dot x+y\dot y}{2}=-\mu r \sin^2\phi(r^2\cos^2\phi-1)$
$\dot \phi=\frac{x\dot y-y\dot x}{r^2}=-1-\mu(r^2\cos^2\phi-1)\cos\phi \sin\phi$.

When $|\mu|\ll 1$, $r$ changes slowly (time scale $\sim 1/\mu$) compared to $\phi$ (time scale $\sim 1$). Introduce a slow, smoothed variable $R$ obtained by filteing out the fast oscillations in $\phi$. Its dynamics is written by averaging the $\dot r$ equation over the fast variable $\phi$.

$\dot R=\frac{1}{2\pi}\int_{0}^{2\pi}d\phi\dot r|_{r\rightarrow R}=\frac{1}{2\pi}\int_0^{2\pi}d\phi[-\mu R\sin^2\phi)(R^2\cos^2\phi-1)]$
$=-\frac{\muR}{8}(R^2-4)$

When $\mu>0$ we have an [[Unstable Fixed Points|unstable fixed point]] at $R=0$ and stable fixed point at $R=2$. Thus, to lowest order in $\mu$ the system has a stable limit cycle of radius $2$. An exact solution of the equation above gives.

$R=\frac{2}{\sqrt{1+(4R_0^{-2}-1)e^{-\mu t}}}$

This is the same result that was obtained for the amplitude when using [[Two-Timing|two-timing]], with $R_0=A(0)=1$