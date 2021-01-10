Melnikov's method can be used to create a homoclinic orbit for damped pendulums by inserting energy into the system.

For a [[Weakly Damped And Weakly Driven Pendulum]]:

![[Weakly Damped And Weakly Driven Pendulum Illustration.png]]
The position of the saddle point is shifted to $(\theta^*,y^*)=(\pi-\text{asin}(I),0)$ (the constant driving shifts the unstable equilibrium from up-side down to an angle).

Evaluate the energy function from the unperturbed system, $H=\frac{y^2}{2}-\cos \theta$, along a trajectory originating from the saddle. For most values of $\alpha$ and $I$ we end up at a point different from the saddle after one lap on the cylinder. Such trajectories have non-zero $\Delta H=H_{\text{end}}-H_{\text{start}}$ ($H$ is assumed to vary smoothly with the small parameters $\alpha$ and $I$)

![[Nonzero Energy Delta On Cylinder Illustration.png]]

The Aim of Melnikov's method is to find the critical small parameters $I$ and $\alpha$ such that $\Delta H=0$ and consequently $\Delta y = 0$ for the perturbed trajectory (*perturbed*=governed by the equation for a [[Driven Damped Pendulum]], with non-zero $\alpha$ and $I$).

The change in $H$ when going from $\theta=-\pi-\text{asin}(I)$ to $\theta=\pi-\text{asin}(I)$ (the sought [[Homoclinic Orbit|homoclinic orbit]]) along a perturbed [[Trajectory|trajectory]] is given by by the *Melnikov Integral* $\Delta H = \int_{-\infty}^{t_f}dt\dot H$  (where the upper integration bound $t_f$ is the time at which $\theta=\pi-\text{asin}(I)$ is reached (assuming $I\ge I_c$ so that $\theta=\pi-\text{asin(I)}$ is reached at all))

$\Delta H = \int_{-\infty}^{t_f}dt\dot H=\int_{-\infty}^{t_f}dt[\underbrace{\dot y}_{-\alpha y - \sin \theta+I}y+\underbrace{\dot \theta}_{y}\sin \theta]$
$=\int_{-\infty}^{t_f}dt y(I-\alpha y)=\int_{-\infty}^{t_f}dt\frac{d\theta}{dt}(I-\alpha y)$
$=\int_{-\pi-\text{asin}(I)}^{\pi-\text{asin}(I)}d\theta(I-\alpha y)=[\text{Use }y=y_h^+=\sqrt{2+2\cos\theta}+O(I,\alpha)]$
$=\int_{-\pi-\text{asin}(I)}^{\pi-\text{asin}(I)}d\theta(I-\alpha\sqrt{2+2\cos \theta})+O(\alpha^2,\alpha I)$
$=2\pi I-8\alpha+O(\alpha^2,\alpha I)$

Thus $\Delta H=0$ is a simple zero for $I_c=4\alpha/\pi+O(\alpha^2)$. We have found an orbit that has the same value of $H$ after one lap on the cylinder, and which is isolated ($\Delta H$ is simple zero, any modificaiton of $I_c$ gives $\Delta H\ne 0$)$\implies$ the found orbit is the sought [[Homoclinic Orbit|homoclinic orbit]]. 

The same evaluation for the lower homoclinic orbit (going from $\theta=\pi-\text{asin}(I)$ to $\theta=-\pi-\text{asin}(I)$) gives $\Delta H=-2\pi I-8\alpha$, i.e.$\Delta H=0$ cannot be satisfied $\implies$ the lower homoclinic orbit is always broken if $\alpha>0$ and $I>0$. In conclusion, for small $\alpha$ and $I$ we have a [[Bifurcation Of Homoclinic Orbit|homoclinic bifurcation]] at $I_c\approx 4\alpha/\pi$
