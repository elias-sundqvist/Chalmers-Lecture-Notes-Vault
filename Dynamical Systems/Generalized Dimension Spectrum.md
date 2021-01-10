---
alias:
  - Generalized Box-Counting Dimension
  - Rényi Dimension Spectrum
---
The [[Box-Counting Dimension]] weighs all boxes  equally.  This is fine for ideal mathematical fractals ([[Cantor Set]], [[Koch Curve]], etc.) But many [[Strange Attractors|stange attractors]] show fluctuations in the occupation number of the boxes: Often a small percentage of boxes are visited frequently, while most boxes are only sparsely visited. Depending on our purpose we may be interested in boxes where trajectories spend more or less time. We therefore introduce a generalized dimension $D_q$ which weigh boxes differently depending on how large fraction of points they contain. 

Noteworthy special cases of the Rényi dimension are 
* $D_0$ is the [[Box-Counting Dimension]]
* $D_1$ is the [[Information Dimension]]
* $D_2$ is the [[Correlation Dimension]]

Let $N_{\text{point}}$ be a large number of points, ideally $N_{\text{point}}\rightarrow\infty$, on a [[Fractal|fractal set]] or [[Strange Attractors|fractal attractor]]. Label $\epsilon$-sized boxes that contain at least one point by $k=1,\dots,N_{\text{box}}(\epsilon)$. Let $p_k(\epsilon)=N_k(\epsilon)/N_{\text{point}}$ be the fraction of points in box $k$. Check normalization:

$\sum_{k=1}^{N_{\text{box}}}p_k=\frac{1}{N_{\text{point}}}\sum_{k=1}^{N_{\text{box}}}N_k=\frac{1}{N_{\text{point}}}=1$

The *generalized dimension* $D_q\equiv\frac{1}{1-q}\underset{\epsilon\rightarrow 0}{\lim}\frac{\ln I(q,\epsilon)}{\ln(1/\epsilon)}$

with a real parameter $q$ and 

$I(q,\epsilon)=\sum_{k=1}^{N_{\text{box}}}p_k^q(\epsilon)$

The significance of $q$ can be summarized as:

* If $q=0$, density variations are neglected. In this limit we recover the [[Box-Counting Dimension]]
   $D_0=\frac{1}{1}\underset{\epsilon\rightarrow 0}{\lim}\frac{\ln I(0,\epsilon)}{\ln(1/\epsilon)}=\underset{\epsilon\rightarrow 0}{\lim}\frac{\ln\left(\sum_{k=1}^{N_{\text{box}}}p_k(\epsilon)^0\right)}{\ln(1/\epsilon)}=\underset{\epsilon\rightarrow 0}{\lim}\frac{\ln\left({N_{\text{box}}}\right)}{\ln(1/\epsilon)}$
* If $q>0$ contributions to $I(q,\epsilon)$ from regions of high density on the attractor are amplified compared to low density regions. $D_q$ with large $q$ therefore characterises clustering of high-density regions.
* When $q<0$ the opposite is true: low-density regions dominate contributions to $I(q,\epsilon)$ and $D_q$

It is possible to show that $D_q$ is a non-growing function of $q$, i.e.
$D_q\ge D_{q'}$ if $q<q'$. 

Typically it looks something like this:

![[Generalized Dimension Spectrum Dq Illustration.png]]

The difference between $D_{-\infty}$ and $D_{\infty}$ determines how large the variations of the [[Fractional Dimensionality|fractal dimension]] are on the [[Strange Attractors|strange attractor]].

* If $D_{-\infty}=D_\infty$, (a flat $D_q$ spectrum) we have a [[Monofractal]] 
* If $D_q$ is not constant with respect to $q$, we have a [[Multifractal]], (so the points are non-uniformly distributed on the fractal)