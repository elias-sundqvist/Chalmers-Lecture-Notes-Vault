A van der Pol oscillator is a type of [[Oscillator With Negative Damping]], but with a non-linear damping factor ($-\mu$ is replaced with $f(x)=\mu(x^2-1)$)
i.e. The formula for a van der Pol oscillator is 

$\ddot x + \underbrace{\mu(x^2-1)}_{f(x)}\dot x+x=0$

Nonlinear damping coefficient $f(x)$ damps large oscillations (friction when $|x>1|$) and amplifies small oscillations (forcing when $|x|<1$).
> Note: It is therefore also called a [[Forced Pendulum With Friction]].
$\implies$ we expect self-sustained oscillations to be possible 

Indeed the corresponding dynamical system

$\dot x = y$
$\dot y =-x-\mu(x^1-1)y$

shows a stable limit cycle if $\mu>0$ (after rescaling $x=x'/\sqrt \mu$ and $y=y'/\sqrt \mu$, the system has a supercritical Hopf bifurcation):

![[Van Der Pol Oscillator Hopf Bifurcation.png]]

Period time and shape of the cycle depends on $\mu$. 

The van der Pol oscillator is an example of a [[Liénard System]]

The van der Pol oscillator can not be solved analytically for general values of $\mu$. In certain limits however, we can find approximate solutions for the limit cycle.

For $\mu \gg 1$,  see [[Relaxation Oscillations]]

Relaxation oscillators have two widely separated time scales acting sequentially. In the opposite  limit $\mu\ll1$ the  situation is more complicated: two time scales act at the same time. See [[Van Der Pol Oscillator With Small Mu]]