---
alias:
  - Relaxation Oscillator
---
![[Relaxation Oscillator Illustration.png]]

Relaxation Oscillators are [[Oscillator|oscillators]] that have very slow build-up and sudden discharge (for example the periodic firing of nerve cells, geysers, [[Stick-Slip Oscillations|stick-slip oscillators]])

Relaxation oscillators have two widely separated time scales acting sequentially. 

### Example Of Relaxation Oscillator:

Consider a [[Van Der Pol Oscillator]] with $\mu\gg 1$.

Let $\epsilon = 1/\mu\ll 1$ be small. Let $y=\epsilon \dot x+F(x)$ with $F(x)=x^3/3-x$:

$\epsilon \dot x = y-F(x)$
$\dot y=\epsilon \ddot x+F'(x)\dot x=-\epsilon x$

Two kinds of dynamics emerge:

Fast: If $|y-F(x)|\sim 1$: $|\dot x|\gg 1$ and $|\dot y|\sim \epsilon\ll 1$
Slow: If $|y-F(x)|\sim \epsilon^2$:$|\dot x|\sim \epsilon$ and $|\dot y|\sim \epsilon$

The dynamics can be understood by plotting the [[Nullclines|nullclines]] $\dot x=0$ $(y=F(x))$ and $\dot y=0$

![[Van Der Pol Relaxation Oscillator Illustration.png]]

Starting at any point (except [[Fixed Points|fixed point]] in origin) the [[Trajectory|trajectory]] moves quickly horizontally onto the cubic [[Nullclines|nullcline]] $y=F(x)$, then it moves slowly close to the [[Nullclines|nullcline]] until the "jump-off points" (max and min of $F(x)$) where the direction of the [[Flow|flow]] and the [[Nullclines|nullcline]] starts to deviate. After the jump-off point the [[Trajectory|trajectory]] quickly moves over to the branch on the opposite side, and so it continues (the red underlying [[Limit Cycle|limit cycle]] is approached.) 

The [[Period Time|period time]] can be approximated by the travel time along the two slow branches. On the slow branches $y\approxF(x)\implies\dot y\approx F'(x)\dot x$.
But we also have $\dot y =-\epsilon x$
$\implies F'(x)\frac{dx}{dt}\approx -\epsilon x$, $\implies dt\approx -\frac{1}{\epsilon x}F'(x)dx$
$\implies T_{\text{slow}}\approx -\int_{x_1}^{x_2}\frac{1}{\epsilon x}F'(x)dx=-\frac 1\epsilon \left[\frac{x^2}{2}-\ln x\right]_{x_1}^{x_2}$
$=\[\text{Take slow branch from \(x_1=2\) to \(x_2=1\)}\]=\frac{1}{2\epsilon}[3-2\ln 2]$

Slow compared to $T_{\text{fast}}\sim \epsilon\implies$ period time is $\approx 2T_{\text{slow}}$ 
