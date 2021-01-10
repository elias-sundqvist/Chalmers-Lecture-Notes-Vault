Using the [[Deformation Matrix|deformation matrix]] $\mathbb M$ it is possible to generalize the [[Maximal Lyapunov Exponent|maximal lyapunov exponent]].

While the [[Maximal Lyapunov Exponent|maximal lyapunov exponent]] describes stretching rates of small separations, it also possible to define the stretching rates of small $K$-dimensional sub-volumes, $\mathcal V_K$, between groups of closeby trajectories for large t:

$\mathcal V_K\sim e^{(\lambda_1+\lambda_2+\dots+\lambda_K)t}\mathcal V_{K,0} \implies \lambda_1+\dots+\lambda_k=\underset{t\rightarrow\infty}{\lim}\;\frac 1 t \ln\left(\frac{\mathcal V_{K}}{\mathcal V_{K,0}}\right)$

(Note that $\sim$ means that the error goes to 0 as $t$ goes to infinity)

Here, $\mathcal V_{K,0}$ denotes a small initial volume and $\lambda_i$ denotes ordered rates $\lambda_1\ge \lambda_2\ge \dots\ge \lambda_n$, defining a *spectrum of [[Lyapunov Exponent|lyapunov exponents]]*

* $\lambda_1$ determines the exponential growth rate ($\lambda_1>0$) or contraction rate ($\lambda_1<0$) of small separations between two trajectories.
* $\lambda_1+\lambda_2$ determines the exponential growth rate $(\lambda_1+\lambda_2>0)$ or contraction rate $(\lambda_1+\lambda_2<0)$ of small areas between three trajectories.
  **Example**: Consider the case $\lambda_1>0,\lambda_2<0$ and $\lambda_1+\lambda_2>0$. A disk of trajectories around the trajectory $\mathbf x(t)$ grows exponentially fast in an unstable direction $\hat{\mathbf u}$ with rate $\lambda_1$ and shrinks exponentially fast along a stable direction $\hat{\mathbf s}$ with rate $\lambda_2$ such that the area increases with exponential rate $\lambda_1+\lambda_2$.
  ![[Lyapunov Spectrum Stretching of 2D Subvolume Example.png]]
* $\lambda_1+\lambda_2+\lambda_3$ determines exponential growth /contraction rate of small volumes between four trajectories.
* and so on for sums over increasing number of Lyapunov exponents.


For calcuating the lyapunov exponents analytically, see [[Analytical Expression Of Lyapunov Exponents]]

For calculating the lyapunov exponents numerically, see [[Numerical Computation Of Deformation Matrix]]