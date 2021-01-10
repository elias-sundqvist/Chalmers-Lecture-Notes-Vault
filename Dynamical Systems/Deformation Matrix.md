---
alias:
  - Deformation Gradient Tensor
  - Lyapunov Matrix
---

![[Deformation Matrix Illustration.png]]

Consider a general [[Flow|flow]] $\dot{\mathbf x}=\mathbf f(\mathbf x)$ and a [[Separation Of Trajectories|separation]] $\mathbf \delta=\mathbf x'-\mathbf x$ with $|\mathbf \delta|\ll 1$ between two trajectories $\mathbf x(t)$ and $\mathbf x'(t)$. 

Here we consider the full linearized dynamics of $\mathbf \delta$.

$\mathbf \delta=\mathbf f(\mathbf x')-\mathbf f(\mathbf x)$
$=[\mathbf \delta \text{ small}\implies \text{ expand }\mathbf f(\mathbf x')\text{ around }\mathbf x]$
$\approx [\mathbf f(\mathbf x)+\mathbb J(\mathbf x)(\mathbf x'-\mathbf x)]-\mathbf f(\mathbf x)=\mathbb J(\mathbf x)\mathbf \delta$

With [[Stability Matrix|stability matrix]] $\mathbb J(\mathbf x)\equiv \frac{\partial \mathbf f}{\partial \mathbf x}$ evaluated along $\mathbf x(t)$.

The deformation matrix $\mathbb M$ is defined such that

$\mathbf \delta(t)=\mathbb M(t)\mathbf \delta(0)$

with small initial separation $|\mathbb \delta(0)|\ll 1$. For a given trajectory $\mathbf x(t)$, $\mathbb M(t)$ transforms an initial separtaion $\mathbf \delta(0)$ to the separation $\mathbf \delta(t)$:


To derive an equation for the evolution of $\mathbf M$, differentiate $\mathbf \delta$ w.r.t. $t$.

$\dot{\mathbf \delta}(t)=\dot{\mathbb M}(t)\mathbb \delta(0)$

and consequently 

$\dot{\mathbb M}(t)\mathbf\delta)(0)=\mathbb J(\mathbf x)\mathbb M(t)\mathbf \delta(0)$.

This equation is true for any initial separation $\mathbf \delta(0)$
$\implies \dot {\mathbb M}(t)=\mathbb J(\mathbf x)\mathbb M (t)$

In summary, to find $\mathbb M(t)$ we need to integrate the joint equations 

$\dot{\mathbf x}=\mathbf f(\mathbf x)$
$\dot{\mathbb M}=\mathbb J(\mathbf x)\mathbb M$

with initial condition $\mathbf x(0)=\mathbf x_0$ and $\mathbb M(0)=\mathbb I$ (identity matrix) for a time long enough that the initial conditions are "forgotten".

The eigenvalues of $\mathbb M$ define the [[Stability Exponents Of Trajectory Separations]]

It is in general hard to solve equations for $\mathbb M$ analytically and one needs to use a numerical method (see [[Numerical Computation Of Deformation Matrix]])