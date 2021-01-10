The [[Separation Of Trajectories|separation of two trajectories]] is given by

$\delta(t)=\delta(0)\exp\left[\int_0^tdt'h(t')\right]$

The maximal Lyapunov exponent is calculated as 
$\lambda_1=\underset{t\rightarrow\infty}{\lim}\;\frac 1t\int_0^tdt'h(t')$

Intuitively, this means that, if we consider large $t$,  the separation of two trajectories can be approximated as 
$\delta(t)\sim\delta(0)e^{t\lambda_1}$ 

(Note that $\sim$ means that the error goes to 0 as $t$ goes to infinity)

This gives us another way of calculating $\lambda_1$

$\lambda_1\equiv \underset{t\rightarrow\infty}\lim\;\frac 1t\frac{|\mathbf \delta(t)|}{|\mathbf \delta(0)|}$

$\lambda_1$ describes whether a system is sensitive to small deviations in initial conditions. Depending on the sign of $\lambda_1$, a small deviation between two trajectories either decreases ($\lambda_1<0$) or increases ($\lambda_1>0$) exponentially fast for large times.


### Physical Interpretation Of $\lambda_1$

A positive $\lambda_1$ (and [[Mixing]]) implies [[Chaotic Systems|dynamics]]. 