There are several ways to define a [[Fractional Dimensionality|fractal dimension]]

One estimate of the dimensionality of an attractor is the Lyapunov dimension $D_L$. It is defined as the number of ordered [[Lyapunov Exponent|lyapunov exponents]] that sum to zero. 

For regular [[Attractor|attractors]]:
* $D_L$ becomes $0$ for the [[Fixed Points|fixed point]]
* $D_L$ becomes $1$ for the [[Limit Cycle|limit cycle]]
* $D_L$ becomes $2$ for the [[Limit Torus|limit torus]]
* $D_L$ becomes $3$ for the [[Volume Conserving System]]

For a [[Strange Attractors|strange attractor]] $D_L$ is typically not an integer. 

For example, for the following strange attractor:

![[Strange Attractor Illustration.png]]
we have
$\lambda_1+\lambda_2>0$ and $\lambda_1+\lambda_2+\lambda_3<0$

The Lyapunov dimension is found by linearly interpolating between the sum of ordered [[Lyapunov Exponent|Lyapunov Exponents]] and choosing the point where the interpolated line is zero. 

![[Lyapunov Dimension Illustration.png]]

$D_L$ is given by a linear interpolation

For three dimensions we have 

$D_L(\lambda_1+\lambda_2)=A+B(\lambda_1+\lambda_2)$ where $A$ and $B$ are determined by $D_L(0)=2$ and $D_L(-\lambda_3)=3$, so 

$D_L=2-\frac{\lambda_1+\lambda_2}{\lambda_3}$

This is a number between $2$ and $3$ as desired (seen from the constraints $\lambda_1+\lambda_2>0$ and $\lambda_1+\lambda_2+\lambda_3<0$ $\implies \lambda_3<-(\lambda_1+\lambda_2)$).

Similarly, the Lyapunov dimension can be generalized to other dimensionalities of phase space. 