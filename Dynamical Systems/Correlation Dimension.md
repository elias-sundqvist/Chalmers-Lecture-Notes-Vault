The correlation dimension is a special case of the [[Generalized Dimension Spectrum]] $D_q$, with $q=2$.

Rewrite 

$I(q=2,\epsilon)=\sum_{k=1}^{N_{\text{box}}}p_k^2=\sum_{k=1}^{N_{\text{box}}}\left(\frac{N_k}{N_{\text{point}}}\right)^2=\frac{1}{N_{\text{point}}^2}\sum_{k=1}^{N_{\text{box}}}N_k^2$
$=\frac{1}{N_{\text{point}}^2}\sum_{k=1}^{N_{\text{box}}}N_k\sum_{\alpha=1}^{N_{\text{point}}}\cases{1&if \(\mathbf x_\alpha\in k\):th box\\0&otherwise}$
$=\frac{1}{N_{\text{point}}^2}\sum_{k=1}^{N_{\text{box}}}\sum_{\beta=1}^{N_{\text{point}}}\sum_{\alpha=1}^{N_{\text{point}}}\cases{1&if \(\mathbf x_\alpha\&\mathbf x_\alpha\in k\):th box\\0&otherwise}$
> $\alpha$ and $\beta$ run over all particles $\implies$ redundant to sum over boxes

$=\frac{1}{N_{\text{point}}^2}\sum_{\beta=1}^{N_{\text{point}}}\sum_{\alpha=1}^{N_{\text{point}}}\cases{1&if \(\mathbf x_\alpha\&\mathbf x_\alpha\in\) same box\\0&otherwise}$
$\sim\frac{1}{N_{\text{point}}^2}\sum_{\beta=1}^{N_{\text{point}}}\sum_{\alpha=1}^{N_{\text{point}}}\cases{1&if \(\mathbf x_\alpha\) within distance \(\epsilon\) from \(\mathbf x_\beta\)\\0&otherwise}$
$=\frac{1}{N_{\text{point}}^2}\sum_{\beta=1}^{N_{\text{point}}}\sum_{\alpha=1}^{N_{\text{point}}}\Theta(\epsilon-|\mathbf x_\alpha-\mathbf x_\beta|)$

This is the *correlation sum*. It describes the probability $P(|\mathbf x_1-\mathbf x_2|<\epsilon)$ to find two point $\mathbf x_1$ and $\mathbf x_2$ on the [[Attractor|attractor]] within distance $\epsilon$.

The correlation dimension $D_C$ can be defined as
$D_2=\frac{1}{1-2}\underset{\epsilon\rightarrow 0}{\lim}\frac{\ln(I(q=2,\epsilon))}{\ln(1/\epsilon)}$
$=\underset{\epsilon\rightarrow 0}{\lim}\frac{\ln(P(|\mathbf x_1-\mathbf x_2|<\epsilon)}{\ln\epsilon}\equiv D_C$

So $D_C$ is defined from the scaling $P(|\mathbf x_1-\mathbf x_2|<\epsilon)\sim  \epsilon^{D_C}$

Note that $D_2$ is often easier to evaluate using the correlation sum than from [[Box-Counting Dimension|box counting]]. It is also what you typically measure in experiments.

Similarly $D_n$ with $n=2,3,4,\dots$ describes scaling of probability to find $n$ particles with separation $\epsilon$,