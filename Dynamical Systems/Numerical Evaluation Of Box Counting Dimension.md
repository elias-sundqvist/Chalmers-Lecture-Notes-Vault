In order to numerically evaluate the [[Box-Counting Dimension]] $D_0$ for a set of numerically evaluated points on a [[Fractal|fratal]], it is not enough to use the box counding dimension formula 

$D_0=\underset{\epsilon\rightarrow 0}{\lim}\;\frac{\ln N_{\text{box}}}{\ln(1/\epsilon)}$ for a small value of $\epsilon$.

* We do not know if we have enough points in our data to resolve the chosen value of $\epsilon$
* Even if $\epsilon$ is small, the scaling law has an unknown coefficient: 
  $N_{\text{box}}=\underbrace{A_0}_{\text{Unknown}}\epsilon^{-D_0}$
  $\implies \ln N_{\text{box}}(\epsilon)=\ln A_0+D_0\ln(1/\epsilon)\rightarrow D_0\ln(1/\epsilon)$ as $\epsilon\rightarrow 0$
  The limit $\epsilon\rightarrow 0$ is slow because of the logarithm. Since we do not know beforehand how large $A_0$ is, we do not know how small $\epsilon$ needs to be to neglect the contribution $\ln A_0$.

Instead, use the slope of the curve $\ln N_{\text{box}}(\epsilon)$ against $\ln \epsilon$ ($A_0$ drops out):

$D_0=-\frac{\Delta \ln N_{\text{box}}(\epsilon)}{\Delta \ln \epsilon}$

Numerical evaluation of the curve typically results in a plot like this:

![[Numerical Box Counting Curve Illustration.png]]