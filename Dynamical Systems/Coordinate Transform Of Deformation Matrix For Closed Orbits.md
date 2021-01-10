At multiples of the [[Period Time|period time]] of a [[Closed Orbit|closed orbit]], the [[Deformation Matrix|deformation matrix]] $\mathbb M$ is (similarity-) invariant under general coordinate transformations. This property can sometimes be useful for [[Analytical Computation Of The Deformation Matrix]]

Start from the equation defining $\mathbb M$ (subscripts denote original coordinates $\mathbf x$), $\mathbf \delta_{\mathbf x}(t)=\mathbb M_{\mathbf x}(t)\mathbf \delta_{\mathbf x}(0)$. Change coordinates $\mathbf x=\mathbf G(\mathbf y)$


![[Coordinate Transformation Of M For Closed Orbits Illustration.png]]

For small seaprations $\mathbf \delta_{\mathbf x}$ and $\mathbf \delta_{\mathbf y}$ we have.

$\mathbf \delta_{\mathbf x}(t)=\frac{\partial \mathbf x}{\partial \mathbf y}\mathbf \delta_{\mathbf y}(t)\equiv\mathbb J_{G}(\mathbf y(t))\mathbf \delta_{\mathbf y}(t)$
$\mathbf \delta_{\mathbf x}(0)=\mathbb J_G(\mathbf y(0))\mathbf \delta_{\mathbf y}(0)$

where $\mathbb J_G$ is the gradient matrix of the transformation $G$. Consequently

$\mathbf \delta_{\mathbf y}(t)=\mathbb J_G^{-1}(\mathbf y(t))\underbrace{\mathbf \delta_{\mathbf x}(t)}_{\mathbb M_{\mathbf x}(t)\mathbf \delta_{\mathbf x}(0)}$
$=\mathbb J_G^{-1}(\mathbf y(t))\mathbb M_{\mathbf x}(t) \mathbb J_G(\mathbf y(0))\delta_{\mathbf y}(0)$
But from the definition of the deformation matrix $\mathbb M_{\mathbf y}(t)$ in the $\mathbf y$-system we also have $\mathbf\delta_{\mathbf y}(t)=\mathbb M_{\mathbf y}(t)\mathbf \delta_{\mathbf y}(0)$

$\implies \mathbb M_{\mathbf y}(t)=\mathbb J_{G}^{-1}(\mathbf y(t))\mathbb M_{\mathbf x}(t)\mathbb J_G(\mathbf y(0))$

For a [[Closed Orbit|closed orbit]] at multiples of the [[Period Time|period time]] (so that $\mathbf y(t)=\mathbf y(0)$) eigenvalues of $\mathbb M_{\mathbf y}=$ eigenvalues of $\mathbb M_{\mathbf x}$. This can be seen by diagonalization. 

$\mathbb M_{\mathbf x}(t)=\mathbb P^{-1}\mathbb D\mathbb P\implies \mathbb M_{\mathbf y}(t)=[\mathbb P\mathbb J_G^{-1}(\mathbf y(0))]^{-1}\mathbb D[\mathbb P \mathbb J_G(\mathbf y(0))]$,
i.e. also $\mathbb M_{\mathbf y}(t)$ is diagonalized with the same diagonal matrix $\mathbb D$.