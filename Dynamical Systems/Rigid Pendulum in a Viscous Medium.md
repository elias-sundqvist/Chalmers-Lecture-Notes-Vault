This is an example derivation of a [[Dynamical System]]

Consider a bead of mass $m$ atached to a massless rod of length $l$ that swings in a vertical plane with angle $\theta$:

![[Rigid pendulum in a viscuous medium illustration.png]]

Three forces act on the bead: 
1. Force from rod acting in negative $\hat r$ direction, $\mathbf F_{\text{rod}}$
2. Downward force from gravity: $\mathbf F_g=-mg\hat {\mathbf y}$.
    Component in radial direction $\hat{\mathbf r}$: $F_{g,r}=mg\cos\theta$ is balanced by force from rod, $F_{g,r}\hat{\mathbf r}=-\mathbf F_{\text{rod}}$
	Component in angular direction $\hat{\mathbf \theta}$ (tangential to pendulum motion): $F_{g,\theta}=-mg\sin \theta$
3. Drag force (dure to friction with the viscous medium, e.g. air), assumed to be proportional to instantaneous velocity in the angular direction: $F_{d,\theta}=-\underbrace{\gamma}_{\text{damping coefficient}}\cdot \underbrace{l\dot \theta}_{\text{tangential velocity }v=l\dot \theta}$

[[Newton's Second Law|Newton's second law]] for angular component of forces $ma=F_{\text{tot},\theta}=F_{g,\theta}+F_{d,\theta}$

Tangential acceleration $a=l\ddot \theta\implies ml\ddot \theta = -mg\sin \theta-\gamma \dot \theta$.


To simplify the analysis we introduce [[Dimensionless Units|Dedimensionalisation]].

Make time dimensionless: $t=t_0t'$, with dimensionless time $t'$ and dimensional constant $t_0$. Using
$\dot \theta = \frac{1}{t_0}\frac{d\theta}{dt'}$ and $\ddot \theta = \frac{1}{t_0^2}\frac{d^2\theta}{dt'^2}$.

gives us $\frac{ml}{t_0^2}\frac{d^2\theta}{dt'^2}=-mg\sin \theta-\frac{\gamma l}{t_0}\frac{d\theta}{dt'}$

Multiply by $\frac{t_0}{\gamma l}$ and choose $t_0=\frac{l\gamma}{mg}$ to remove all parameter dependence on the right hand side:
$\frac{m}{t_0\gamma}\frac{d^2\theta}{dt'^2}=-\frac{mgt_0}{\gamma l}\sin \theta-\frac{d\theta}{dt'}=\left[t_0=\frac{l\gamma}{mg}\right]=-\sin\theta-\frac{d\theta}{dt'}$.

To simplify the notation we replace $t'$ with $t$ from now on. We have.
$\epsilon \ddot \theta = - \sin \theta-\dot \theta$ where $\epsilon \equiv \frac{m}{t_0\gamma}$. Assume large damping $(\epsilon\rightarrow 0)$ to obtain a one-dimensional dynamical system $\dot \theta=-\sin \theta$.

This equation is non-linear but solvable by [[Separation of Variables|separation of variables]] 

$\frac{1}{\sin \theta}d\theta=-dt$

Integrate from $t=0$ to $T$ and from $\theta(0)\equiv \theta_0$ to $\theta(T)\equiv \theta_T$
$I=\int_{\theta_0}^{\theta_T}\frac{1}{\sin \theta}d\theta=-\int_0^Tdt=-T$

$I=\int_{\theta_0}^{\theta_T}\frac{2i}{e^{i\theta}-e^{-i\theta}}d\theta=\int_{\theta_0}^{\theta_T}\frac{2ie^{i\theta}}{e^{2i\theta}-1}d\theta=\left[z=e^{i\theta},dz=ie^{i\theta}d\theta\right]$
$=\int \frac{2}{z^2-1}dz=\left[\text{partial fraction decomposition}\right]$
$=\int \left(\frac{1}{z-1}-\frac{1}{z+1}\right)dz=\left[\ln\left(\frac{e^{i\theta}-1}{e^{i\theta}+1}\right)\right]_{\theta_0}^{\theta_T}=\left[\ln\left(\tan\left(\frac \theta 2\right)\right)\right]_{\theta_0}^{\theta_T}$

In conclusion
$\ln\left(\frac{\tan\left(\frac{\theta_T}{2}\right)}{\tan\left(\frac{\theta_0}{2}\right)}\right)=-T\implies \theta(t)=2\text{atan}\left(e^{-t}\tan\left(\frac{\theta_0}{2}\right)\right)$

Trajectories starting with $-\pi<\theta_0<\pi$ converge to $\theta=0$ as $t\rightarrow \infty$
Trajectories staring at $\theta_0=\pm \pi$ remain at $\pm \pi$.

![[Fully damped pendulum trajectories.png]]

**Solution using a dynamical systems approach**
It is easier to solve the system geometrically. Plot $\dot \theta=f(\theta)$ against $\theta$:

![[Full Damped pendulum dynamical systems approach.png]]

Arrows denote directions along the line.
Points with no flow $(\dot \theta=0)$ are called [[Fixed Points|fixed points]]

The [[Geometrical Approach|geometric solution]] gives the qualitative picture: all trajectories end up at $\theta=0$ (or multiples of $2\pi$), unless they start exactly at an [[Unstable]] fixed point. Some details are missing but often it is enought o have qualitative information about the solution. 


Let's go back and consider the equation $\ddot \theta=-\frac g l \sin \theta-\frac{\gamma}{m}\dot \theta$.

Consider small oscillations, $\sin \theta\approx\theta$, and write as a dynamical system with $x=\theta,y=\dot\theta$
$\dot x=y$
$\dot y = -\frac{g}{l}x-\frac{\gamma}{m}y$

This is an examples of a [[Linear 2D Flows|2d linear flow]]. It has a [[Fixed Points|fixed point]] at $x^*=y^*=0$.
As for one-dimensional systems we can do a [[Geometrical Approach|geometrical visualization]] of a few representative [[Trajectory|trajectories]] ([[Phase Portrait|phase portrait]]) to understand the dynamics close to a fixed point. 

![[Rigid Pendulum In Viscous Medium Phase Portrait.png]]

From the [[Phase Portrait|phase portrait]] we find that there are 2 relevant cases. 

* **Case $\gamma=0$**: The [[Fixed Points|fixed point]] is surrounded by [[Closed Orbit|closed orbits]] in the form of ellipses of indinite density (which orbit is chosen depends on the [[Initial Condition]]). The fixed point is a [[Center|center]]. Physical interpretation: The fixed point $x^*=y^*=0$ corresponds to the pendulum at rest, $\theta=\dot \theta=0$. Non-zero initial conditions give closed orbits, corresponding to oscillations in the underlying dynamics.
> The ellipses are formed by the explicit solution $(x,y)=(\theta,\dot \theta)=A_0(\cos(\omega_0t+\phi_0),-\omega_0\sin(\omega_0 t+\phi_0))$ with  $\omega_0=\sqrt{\frac g l}$

* **Case $\gamma>0$**: The [[Fixed Points|fixed point]] is a [[Stable Spiral|stable spiral]] - trajectories spiral inward towards the [[Fixed Points|fixed point]]. Physical Interpretation: Due to the viscous damping $(\gamma>0)$ the magnitude of oscillations decreases with time. 



Doing [[Classification Of Linear Flows|classification of linear flows]] on this system gives us 

$\mathbb A=\begin{bmatrix}0&1\\-\frac g l &-\frac \gamma m\end{bmatrix}$

We have $\tau=-\frac \gamma m$, $\Delta = \frac g l$.

* **Case $\gamma=0$**:
   $\lambda_1=i\sqrt{\frac g l}$, $\lambda_2=-i\sqrt{\frac g l}$. This fixed point is a [[Center|center]], and therefore the [[Eigenvalue|eigenvalues]] are imaginary and the values correspond to the [[Angular Frequency|angular frequency]] $\omega_0=\sqrt{g/l}$.
* **Case $\gamma>0$ but small**:
   $\lambda_1=\frac{-\gamma/m+i\sqrt{4g/l-(\gamma/m)^2}}{2}=-\frac{\gamma}{2m}+i\sqrt{\frac g l-\frac{\gamma^2}{2 m^2}}$
   $\lambda_2=\frac{-\gamma/m-i\sqrt{4g/l-(\gamma/m)^2}}{2}=-\frac{\gamma}{2m}-i\sqrt{\frac g l -\frac{\gamma^2}{2m^2}}$
   This [[Fixed Points|fixed point]] is a [[Stable Spiral|stable spiral]]. It shows oscillating behaviour with [[Angular Frequency|angular frequency]] $\sqrt{\frac g l -\frac{\gamma^2}{2m^2}}$. The negative real part of the [[Eigenvalue|eigenvalues]] decreases the magnitude of the oscillations exponentially with time. 