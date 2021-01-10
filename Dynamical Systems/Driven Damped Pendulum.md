Add a constant torque $\tau$ to the damped pendulum from [[Rigid Pendulum in a Viscous Medium|this example]].

$\ddot \theta=-\frac{\gamma}{m}\dot \theta-\frac{g}{l}\sin \theta+\frac{\tau}{I_0}$ 

with $I_0$ being the moment of intertia.

This equation can be written as a [[Dimensionless Units|dimensionless]] dynamical system by a suitable rescaling of $t$ and $\dot \theta$. In dimensionless units we have:

$\dot \theta=y$

$\dot y=-\alpha y\sin \theta+\underbrace{\frac{\tau l}{I_0 g}}_{I}$

where $\alpha$= [[Dimensionless Units|dimensionless]] damping, $I$= [[Dedimensionalisation|dimensionless]] torque.

Using numerical simulations one obtains a [[Phase Diagram]]

![[Phase Diagram Of Damped Driven Pendulum.png]]

Here lines show bifuractions, black text denots system attractors. 

This system is identical to that of the phase difference in a [[Josephson Junction]]. It can also be used as a lowest-order approximative model for a large number of problems. We can view the system as a [[Flows On The Cylinder|flow on a cylinder]] with $\theta$ periodic $-\pi<\theta\le\pi$ and keep aperiodic angular velocity $y$.

### Analysis for small $\alpha$ and $I$
#### Case: $\alpha=I=0$
When $\alpha=I=0$, the system simplifies to a [[Simple Pendulum|simple (undamped, undriven) pendulum]]. 

This is a [[Hamiltonian Systems|hamiltonian system]] with $V'(\theta)=\sin \theta\implies$ [[Potential]] energy $V(\theta)=-\cos \theta$. On the cylinder there are two distinct [[Fixed Points|fixed points]] given by the potential minimum at $(\theta^*,t^*)=(0,0)$ (nonlinear center) and the potential maximum at $(\theta^*,y^*)=(\pi,0)$ (saddle).

For the simple pendulum, two [[Homoclinic Orbit|homoclinic orbits]] (homoclinic because $(\theta^*,t^*=(-\pi,0))$ and $(\theta^*,y^*)=(\pi,0)$ are the same point on the cylinder) separate regions with closed orbits in the forms of [[Librations|librations]] and [[Rotations|rotations]]

![[Simple Pendulum Homoclinic Orbit Separatrix.png]]

Which orbit is obtain depends on the energy $E$ of the initial condition. 

Along any trajectory we have the dimensionless energy $E=y^2/2-\cos \theta=\text{const}$. (Conservation of energy in [[Hamiltonian Systems|Hamiltonian systems]]). At the saddle point $(\theta^*,y^*)=(-\pi,0)$ we ahve $E=1$, the energy for the [[Homoclinic Orbit|homoclinic orbits]].

[[Librations]] have $E<1$ and [[Rotations|rotations]] $E>1$. Due to energy conservation, $E=y^2/2-\cos t\theta=1$, the two homoclinic orbits can be parameterized as $y_h^{\pm}=\pm\sqrt{2+2\cos \theta}$.

#### Case: $0<\alpha\ll 1$ and $I=0$

When $0<\alpha\ll1$ and $I=0$ we have a [[Weakly Damped Pendulum|weakly damped pendulum]]: The [[Homoclinic Orbit|homoclinic orbits]] are broken and the fixed point $(\theta^*,y^*)=(0,0)$ becomes a stable spiral 
$(\lambda_{1,2=-\alpha/2\pm i\sqrt{1-\alpha^2/4}})$.

Letting $\alpha>0$ destroys the homoclinic orbit due to the dissipative damping term. Is it possible to recover the homoclinic orbit by input of energy from the driving term, $I>0$? Yes! By [[Melnikov's Method]]

#### Case: General small values of $\alpha$ and $I$

For general values of $\alpha$ and $I$ the system has fixed points where $y^*=0$ and $\sin\theta^*=I$. Depending on the value of $I$ we have $0$ ($I>1$), $1$ ($I=1$), or $2$ ($0\le I<1$) [[Fixed Points|fixed points]].

When the driving is weak, ($0<I\ll 1$), we get a [[Weakly Damped And Weakly Driven Pendulum]].

![[Weakly Damped And Weakly Driven Pendulum Illustration.png]]

To find parameters $I$ and $\alpha$ such that a [[Homoclinic Orbit|homoclinic orbit is recovered]], use [[Melnikov's Method]].

What we find when analzing the system using [[Melnikov's Method]] is that there is a [[Bifurcation Of Homoclinic Orbit|homoclinic bifurcation]] at $I_c\approx 4\alpha/\pi$:

![[Homoclinic Bifurcation Of Damped Driven Pendulum.png]]

For $I<I_c$ the damping overtakes the driving and the motion is damped to zero. 

At $I=I_c$ a limiting trajectory (the [[Homoclinic Orbit|homoclinic orbit]]) is created that allows the pendulum to make one full lap, but in infinite time. 

For $I>I_c$ the system is [[Bistable System|bistable]], it shows a [[Stable Limit Cycle|stable limit cycle]] (full lap rotations) and a stable spiral decaying the motion to zero. Which [[Attractor|attractor]] is reached depends on whether the initial position is in the [[Stable Manifold|basin of attraction]] of the [[Limit Cycle|limit cycle]] (green hashed area above) or the [[Spiral|spiral]] (blue hashed), separated by the [[Stable Manifold|stable]]/[[Unstable Manifold|unstable]] [[Manifold Stability|manifolds]] of the [[Saddle Point|saddle point].]

#### Case: Larger $\alpha$ and $I$

When $I>1$ no fixed points exists. [[Librations|librations]] are not possible ([[Index Theory]]: [[Closed Orbit|Closed orbits]] must encircle a [[Fixed Points|fixed point]]). It is possible to show that a unique attracting [[Limit Cycle|limit cycle]] in the form of a rotation exists (the strong torque gives the pendulum a stationary full-lap rotation). For larger values of $\alpha$ it is possible to show that the [[Limit Cycle|limit cycle]] forms in an [[Infinite-Period Bifurcation|infinite time biurcation]], i.e. not a [[Bifurcation Of Homoclinic Orbit|homoclinic bifurcation]] as for small values of $\alpha$.

