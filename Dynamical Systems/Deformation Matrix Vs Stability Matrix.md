The linearization between closeby trajectories, as used for the [[Deformation Matrix|deformation matrix]]. Bears a lot of resemblence to the linearization around [[Fixed Points|fixed points]] used when computing the [[Stability Matrix|stability matrix]].

Stability analysis of separation:
* [[Fixed Points|Fixed Point]]: $\mathbf \delta = \mathbf x-\mathbf x^*$
* [[Deformation Matrix|Trajectory Separation]]:  $\mathbf \delta = \mathbf x'-\mathbf x$

Dynamics ($\dot{\mathbf \delta}=\mathbb J\mathbf\delta$)
* [[Fixed Points|Fixed Point]]: $\mathbb J(\mathbf x^*)$ const.
* [[Deformation Matrix|Trajectory Separation]]:  $\mathbb J(\mathbf x(t))$ along $\mathbf x(t)$

Solution ($\mathbf \delta(t)=\mathbb M(t)\mathbf \delta(0)$)
* [[Fixed Points|Fixed Point]]: $\mathbb M(t)=\exp[\mathbb J(\mathbf x^*)t]$
* [[Deformation Matrix|Trajectory Separation]]:  $\mathbb M$ implicit from trajectory integration

Stability Exponents
* $\sigma_i=\underset{i}{\text{eig}}(\mathbb J(\mathbf x^*))$
* $\overset \sim \sigma_i=\underset{t\rightarrow \infty}{\lim}\frac 1 t\ln(\underset{i}{\text{eig}})(\mathbb M)$


As a consequence, [[Trajectory|trajectories]] in the [[Stable Manifold|basin of attraction]] of a [[Stable Fixed Points|fixed point attractor]] $\mathbf x^*$ have $\mathbf x(t)\rightarrow \mathbf x^*$ for large times and $\mathbb M\rightarrow \text{exp}[\mathbb J(\mathbf x^*)t]$.

Diagonalization of $\mathbb J(\mathbf x^*)=\mathbb P\mathbb D\mathbb P^{-1}$ implies diagonalization of $\mathbb M: \mathbb M=\mathbb P e^{\mathbb Dt}\mathbb P^{-1}$ $\implies$ the [[Eigenvector|eigenvectors]] of $\mathbb M$ and $\mathbb J$ are the same. In this limit the [[Stability Exponents Of Trajectory Separations|stability exponents of separations]] are equal to the [[Stability Exponent|stability exponents]] $\sigma_i$ of a [[Fixed Points|fixed point]] (eignvalues of $\mathbb J(\mathbf x^*)$), $\overset \sim \sigma_i=\sigma_i$. 

In general, the eigenvalues and egienvectors of $\mathbb M$ are different form the eigenvalues  and eigenvectors of $\mathbb J$ (eigensystem of $\mathbb J$ requires only local knowledge of system while eigensystem of $\mathbb M$ is influenced by all stability matrices along a trajectory).
