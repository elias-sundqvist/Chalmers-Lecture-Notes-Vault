The information dimension can be seen as a special case of the [[Generalized Dimension Spectrum]] $D_q$, where $q=1$.

The expression for $D_q$ 

$D_q\equiv\frac{1}{1-q}\underset{\epsilon\rightarrow 0}{\lim}\frac{\ln I(q,\epsilon)}{\ln(1/\epsilon)}$

diverges as $q\rightarrow 1$, so we need to take the limit. 

First expand $\ln I(q,\epsilon)$ around $q=1$

$\ln I(q,\epsilon)=\ln\left(\sum_{k=1}^{N_{\text{box}}}p_k^q\right)$

> Use $p_k^q=p_kp_k^{q-1}=p_k\exp((q-1)\ln p_k)\approx p_k(1+(q-1)\ln p_k)$ for $q\approx 1$

$=\ln\left(\sum_{k=1}^{N_{\text{box}}}p_k+\sum_{k=1}^{N_{\text{box}}}p_k(q-1)\ln p_k)\right)$

> Use norm $\sum_{k=1}^{N_{\text{box}}}p_k=1$ and expand $\ln(1+(q-1)A)\approx (q-1)A$ for $q\approx 1$

$=(q-1)\sum_{k=1}^{N_{\text{box}}}p_k\ln p_k$

We get 

$\underset{q\rightarrow 1}{\lim}D_q=\underset{q\rightarrow 1}{\lim}\underset{\epsilon\rightarrow 0}{\lim}\frac{1}{1-q}\frac{\ln(I(q,\epsilon))}{\ln(1/\epsilon)}$
$=\underset{q\rightarrow 1}{\lim}\underset{\epsilon\rightarrow 0}{\lim}\frac{1}{1-q}\frac{(q-1)\sum_{k=1}^{N_{\text{box}}}p_k \ln p_k}{\ln(1/\epsilon)}$
$=\underset{\epsilon\rightarrow 0}{\lim}\frac{\sum_{k=1}^{N_{\text{box}}}p_k \ln p_k}{\ln(\epsilon)}$