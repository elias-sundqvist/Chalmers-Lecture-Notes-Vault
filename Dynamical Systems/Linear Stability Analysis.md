See [[2D Linear Stability Analysis]] for linear stablity analysis in more than one dimension.

One type of [[Analytical Analysis|analytical]] approach of studying [[Fixed Points|fixed points]] is called linear stability analysis.

Consider a general [[Flow|flow]], $\dot x = f(x)$, with a [[Fixed Points|fixed point]] $x=x^*: f(x^*)=0$.
A small deviation $\eta(t)=x(t)-x^*$ from the fixed point $x^*$ evolves according to $\dot \eta = \dot x- \frac{d}{dt}x^*=\dot x = f(x)$.

Series expand the flow around the fixed point:
$\dot \eta=f(x)=\underbrace{f(x^*)}_{=0}+f'(x)\underbrace{(x-x^*)}_{=\eta}+\frac 12 f''(x^*)\underbrace{(x-x^*)^2}_{=\eta^2}+\dots\approx f'(x^*)\eta$.
Solution: $\eta=\eta_0e^{f'(x^*)t}$.

This is the general form of the solution close to an [[Isolated Fixed Point|isolated fixed point]].
$\lambda=f'(x^*)$ is the [[Stability Exponent|stability exponent]] (a constant number. ) Note that when $\lambda < 0$ the deviation from the [[Fixed Points|fixed point]]  decreases exponentially fast, but the fixed point is not reached ($\eta = 0$) in a finite time. 

