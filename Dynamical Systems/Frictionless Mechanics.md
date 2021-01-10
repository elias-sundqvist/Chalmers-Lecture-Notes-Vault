**Frictionless Mechanics**

If the force $F$ is conservative (e.g. no friction), it can be written as the negative gradient of a scalar [[Potential]] $V(x)$:
$F=-\frac{\partial V}{\partial x}$.

Then [[Newton's Second Law|Newton's law]] can be written as the following dynamical system (introduce momentum $p\equiv m\dot x$)
$\dot x = \frac{p}{m}$
$\dot p=-\frac{\partial V}{\partial x}$

This is an example of a [[Hamiltonian Systems|Hamiltonian system]].

Proof: 
choose $H$ to be the Hamiltonian $H=\frac{p^2}{2m}+V(x)$
to get 
$\dot x = \frac{\partial H}{\partial p}=\frac{p}{m}$
$\dot p = -\frac{\partial H}{\partial x}=-\frac{\partial V}{\partial x}$.

In conclusion, Newton's law with a conservative force is one example of a [[Hamiltonian Systems|Hamiltonian dynamical system]].

In this case, the energy, $E=H(x,p)$ is a conserverved quantity ([[Integral Of Motion]]). This can be verified as follows:

$\dot H=\frac{\partial H}{\partial x}\underbrace{\dot x}_{\frac{\partial H}{\partial p}}+\frac{\partial H}{\partial p}\underbrace{\dot p}_{-\frac{\partial H}{\partial x}}=0$