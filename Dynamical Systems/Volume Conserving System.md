A [[Dynamical System|dynamical system $\dot{\mathbf x}=\mathbf f(\mathbf x)$]] is volume conserving in [[Phase Space|phase-space]] if $\nabla \cdot \mathbf f(\mathbf x)=0$ everywhere.

Consider a [[Phase Space|phase-space]] volume $\mathcal V(t)$ with shape $D(t)$:

![[Volume Conserving Deformation Illustration.png]]

In a volume conserving system a [[Phase Space|phase-space]] element changes shape $D(t)$, but the volume $\mathcal V(t)$ is constant. 

To show this, take a small time step $\delta t$. Positions evolve according to 

$\mathbf x(\delta t)=\mathbf x(0)+\delta t\mathbf f(\mathbf x(0))$

The coordinate transformation $\mathbf y\equiv \mathbf x(\delta t)$ transforms all coordinates $\mathbf x_0\in D(0)$ into the coordinates $\mathbf y\in D(\delta t)$

$\mathcal V(\delta t)=\int_{D(\delta t)}d^{n}y=\int_{D(0)}d^n x_0\left|\det\left(\frac{\partial \mathbf y}{\partial \mathbf x_0}\right)\right|$
$=\int_{D(0)}d^n x_0\underbrace{|\det (1+\delta t\mathbb J(\mathbf x_0))|}_{\approx 1+\delta t\text{Tr}\mathbb J(\mathbf x_0)}=\mathcal V(0)+\delta t \int_{D(0)}d^n x_0\underbrace{\text{Tr}\mathbb J(\mathbf x_0)}_{\nabla\cdot \mathbb f(\mathbb x_0)}$
$\implies \frac{d\mathcal V}{dt}=\int_{D(t)}d^n x\nabla \cdot \mathbf f(\mathbf x)$

If $\nabla \cdot \mathbf f(\mathbf x)=0$ everywhere. $\mathcal V(t)$ is constant and the system is volume conserving.

Volume conserving systems cannot have [[Attractor|Attractors]] nor [[Unstable Fixed Points|Repellers]]

#### Example
Consider the system introduced [[Nonlinear Stability Analysis#Non-Linear Analysis Example|here]]

$\dot x = -y+ax(x^2+y^2)\equiv f(x,y)$
$\dot y =x+ay(x^2+y^2)\equiv g(x,y)$

with a single [[Fixed Points|fixed point]] at $(0,0)$. Evaluate the [[Divergence Of Flow|phase-space contraction]]. 

$\nabla \cdot \mathbf f=\frac{\partial}{\partial x}[-y+ax(x^2+y^2)]+\frac{\partial}{\partial y}[x+ay(x^2+y^2)]=3a(x^2+y^2)$

If $a<0$, the system is [[Dissipative System|dissipative]] and has an [[Attractor|attractor]]. The [[Fixed Points|fixed point]] is a stable spiral. 

If $a>0$ the [[Fixed Points|fixed point]] must be an unstable spiral. When $a=0$, $\nabla \cdot \mathbf f=0$ everywhere $\implies$ the system is [[Volume Conserving System|volume conserving]], so cannot have [[Stable Fixed Points|attractors]] or [[Unstable Fixed Points|repellers]] and the [[Fixed Points|fixed point]] is a [[Center|center]].

