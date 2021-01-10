It is in general hard to solve equations for $\mathbb M$ analytically and one needs to use a numerical method

#### The Naïve Approach 

To numerically calculate the [[Lyapunov Exponent|Lyapunov exponents]] the naïve approach is to solve the dynamical system $\dot {\mathbf x} = \mathbf f(\mathbf x)$ numerically for two trajectoreis starting at $\mathbf x(0)$ and $\mathbf x(0)+\mathbf \delta(0)$.

![[Naïve Approach Of Calculating Maximal Lyapunov Exponent Illustrated.png]]

Since the separation must remain small, rescale the separation vector to original length at regular time intervals $T$.

$\mathbf \delta (nT)\rightarrow \frac{1}{\alpha_n}\mathbf \delta(nT)$, $\alpha_n=\frac{|\mathbf \delta(nT)|}{|\mathbf \delta(0)|}$
and use scaling factors $\alpha_n$ to evaluate 

$\lambda_1=\frac 1 t \ln\frac{|\mathbf \delta(t)|}{|\mathbf \delta(0)|}=\frac{1}{NT}\sum_{n=1}^N\ln\alpha_n$

with the total number of rescaling, $N$, large. 

This often works! But it is unreliable: what are good values for $|\mathbf \delta(0)|$ and $T$? ANother problem is that the method does not give the stretching rate in directions other than the maximal, needed to calculate $\lambda_2,\dots,\lambda_n$. In order to calculate these, one would need to follow $n+1$ trajectories and rescale and reorthonormalize the volume spanned between the trajectories. This is quite complicated

#### Evaluation Using The [[Deformation Matrix]]

In principle, the Lyapunov exponents can be obtained from the equation

$\lambda_i=\underset{t\rightarrow\infty}{\lim}\;\frac 1t \ln|\mathbb R_{ii}|$ (See [[Analytical Expression Of Lyapunov Exponents]])

However, it relies on the integration of the system

$\dot{\mathbf x}=\mathbf f(\mathbf x)$
$\dot{\mathbb M}=\mathbb J(\mathbf x)\mathbb M$

(See [[Deformation Matrix]])

But this integration is generally numerically problematic (the elements in $\mathbb M$ blow up exponentially with increasing $t$). A workaround is obtained by first discretizing time $t\rightarrow t_n\equiv n\delta t$ (where $n$ is an integer and $\delta t$ is a small timestep)

$\frac{\mathbb M(t_n)-\mathbb M(t_{n-1})}{\delta t}=\mathbb J(\mathbf x(t_{n-1}))\mathbb M(t_{n-1})$
$\implies \mathbb M(t_n)$
$=[\mathbb I+\mathbb J(\mathbf x(t_{n-1}))\delta t]\mathbb M(t_{n-1})$
$=[\mathbb I+\mathbb J(\mathbf x(t_{n-1}))\delta t][\mathbb I+\mathbb J(\mathbf x(t_{n-2}))\delta t]\mathbb M(t_{n-2})$
$=[\mathbb I+\mathbb J(\mathbf x(t_{n-1}))\delta t][\mathbb I+\mathbb J(\mathbf x(t_{n-2}))\delta t]\dots[\mathbb I+\mathbb J(\mathbf x(t_{0}))\delta t]\underbrace{\mathbb M(t_{0})}_{=\mathbb I}$

i.e. $\mathbb M(t_n)$ consists of a product of $n$ matrices $\mathbb M(t_n)=\mathbb M^{(n-1)}\mathbb M^{(n-2)}\dots\mathbb M^{(0)}$

The time evolution of the deformation matrix $\mathbb M$ is driven by the stability matrixes $\mathbb J(\mathbf x(t_n))$ along a trajectory $\mathbf x(t)$:

![[Time Evolution Of Deformation Matrix Illustration.png]]

Arrows show eigensystems of $\mathbb M$ (green) and $\mathbb J$ (red). At each time step, the eigendirections of $\mathbb M$ strive against the maximal direction of $\mathbb J$ and become longer if the maximal eigenvalue of $\mathbb J$ is positive $\implies$  Eigenvectors of $\mathbb M$ tend to become very long and almost aligned. $\implies$ hard numerics.

#### Numerical Evaluation Using The [[Deformation Matrix]] and [[QR-Decomposition]]

we evaluate the [[QR-Decomposition]] of $\mathbb M(t_n)=\mathbb M^{(n-1)}\mathbb M^{(n-2)}\dots\mathbb M^{(0)}$ without numerical overflow as follows.

* Before the first time step, QR-decompose $\mathbb M^{(0)}=\mathbb Q^{(0)}\mathbb R^{(0)}$, i.e. $\mathbb Q^{(0)}=\mathbb R^{(0)}=\mathbb I$ because $\mathbb M^{(0)}=\mathbb I$
* After the first time step, rewrite $\mathbb M^{(1)}\mathbb M^{(0)}=\underbrace{\mathbb M^{(1)}\mathbb Q^{(0)}}_{\mathbb Q^{(1)}\mathbb R^{(1)}}\mathbb R^{(0)}=\mathbb Q^{(1)}\mathbb R^{(1)}\mathbb R^{(0)}$
* After the second time step, rewrite $\mathbb M^{(2)}\mathbb M^{(1)}\mathbb M^{(0)}=\underbrace{\mathbb M^{(2)}\mathbb Q^{(1)}}_{\mathbb Q^{(2)}\mathbb R^{(2)}}\mathbb R^{(1)}\mathbb R^{(0)}=\mathbb Q^{(2)}\mathbb R^{(2)}\mathbb R^{(1)}\mathbb R^{(0)}$
* Repeat for each time step: $\mathbb M^{(n-1)}\dots\mathbb M^{(0)}=\mathbb Q^{(n-1)}\mathbb R^{(n-1)}\dots\mathbb R^{(1)}\mathbb R^{(0)}$

In conclusion, we have a [[QR-Decomposition]] $\mathbb M(t_n)=\mathbb Q\mathbb R$, where $\mathbb Q=\mathbb Q^{(n-1)}$ and $\mathbb R=\mathbb R^{(n-1)}\dots\mathbb R^{(1)}\mathbb R^{(0)}$.

Recall that we can use the equation

$\lambda_i=\underset{t\rightarrow\infty}{\lim}\;\frac 1t \ln|\mathbb R_{ii}|$ (See [[Analytical Expression Of Lyapunov Exponents]])

to compute the Lyapunov exponents

For the final time step $N$ we get
$\lambda_i=\underset{N\rightarrow\infty}{\lim}\;\frac{1}{N\delta t}\ln|\mathbb R_{ii}|=\underset{N\rightarrow\infty}{\lim}\;\frac{1}{N\delta t}\sum_{n=0}^{N-1}\ln|\mathbb R_{ii}^{(n)}|$

The $\ln|\mathbb R_{ii}^{(n)}|$ terms can be added one at a time to avoid overflow. 

Implementation Recipe:

1. Solve the equation $\dot{\mathbb x}=\mathbb f(\mathbb x)$ for some time to end up close to the fractal [[Attractor|attractor]].
2. Start with matrix $\mathbb Q=\mathbb I$ and zero-valued variables $\lambda_i$ for the sums. 
3. At each time step you get a new matrix $M^{(n)}=\mathbb I+\mathbb J(\mathbf x(t_n))\delta t$ where $\mathbf x(t_n)$ is taken from the solution of the $\dot{\mathbf x}=\mathbf f(\mathbf x)$ equation.
4. At each time step [[QR-Decomposition|QR-Decompose]] $\mathbb M^{(n)}\mathbb Q_{\text{old}}=\mathbb Q_{\text[new}]}\mathbb R_{\text{new}}$
    > Note: `QRDecomposition[M]` in Mathematica gives matrixes named $Q$ and $R$, but $\mathbb M=\mathbb Q^T\mathbb R$, i.e. one must transpose $\mathbb Q$.
5. At each time step add the log abs diagonal elements of $\mathbb R_{\text{new}}$ to $\lambda_i$.
6. REpeat from step 3 with $\mathbb Q=\mathbb Q_{\text{new}}$ (total of N iterations) 