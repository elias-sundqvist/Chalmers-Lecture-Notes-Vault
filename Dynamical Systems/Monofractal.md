A [[Fractal|fractal]] with a flat [[Generalized Dimension Spectrum]], $D_{-\infty}=D_\infty$ is called a *monofractal*.

In practice, we get a *monofractal* if all regions of the fractal have equal density. 
In other words, points are evenly distributed on the fractal.

(Examples of monofractals are the regular and asymmetric [[Cantor Set|Cantor sets]])

Every point on the attractor is equally likely $\implies D_q=D_0=\text{const}$
which can easily be verified as follows:

$D_q=\frac{1}{1-q}\underset{\epsilon \rightarrow 0}{\lim}\frac{\ln\left(\sum_{k=1}^{N_{\text{box}}}p_k^q\right)}{\ln(1/\epsilon)}$

> Every point equally likely $\implies$ $\underbrace{p_k\sim1/N_{\text{box}}}_{\text{if }\epsilon\rightarrow 0}$ and $\sum_{k=1}^{N_{\text{box}}}=N_{\text{box}}$

$=\frac{1}{1-q}\underset{\epsilon \rightarrow 0}{\lim}\frac{\ln(N_{\text{box}}(1/N_{\text{box}})^q)}{\ln(1/\epsilon)}$
$=\frac{1}{1-q}\underset{\epsilon \rightarrow 0}{\lim}\frac{\ln(N_{\text{box}}^{1-q})}{\ln(1/\epsilon)}$
$=\underset{\epsilon \rightarrow 0}{\lim}\frac{\ln(N_{\text{box}})}{\ln(1/\epsilon)}=D_0$