See [[Cantor Set]]

In the assymetric cantor set, each iteration removes segments of different size (assymetric) from the remaining segments.

For example, here we construct a [[Cantor Set|Cantor set]] by always removing the second quarter:

![[Assymetric Cantor Set Illustration.png]]

Use $\epsilon_k=4^{-k}$. 

> Note:
> From the symmetric Cantor set one could assume $N_{\text{box}}=3^k$, BUT we need to iterate until the largest connected interval is smaller than $\epsilon_k=4^{-k}$ (the set is defined as $n\rightarrow \infty$). To show that $N_{\text{box}}\ne 3^k$, cover successive generations of the set.
> Case $\epsilon_1=4^{-1}$:
> ![[Asymmetric Cantor Set Wrong Approach First Box Size.png]]
> $\implies N_{\text{box}}(\epsilon=1/4)=3$
> Case $\epsilon_2=4^{-2}$:
> ![[Asymmetric Cantor Set Wrong Approach Second Box Size.png]]
> $\implies N_{\text{box}}(\epsilon=1/4^2)=8$, i.e. $N_{\text{box}}(\epsilon=1/4^2)\ne3^2=9$
> In conclusion we must iterate to a generation $n>k$ for the asymmetric Cantor set. The reason is that the asymmetric Cantor set is constructed from two relative length scales.

The asymmetric Cantor set is constructed from two relative length scales $\lambda_a=\frac 14$ and $\lambda_b=\frac 12$

![[Asymmetric Cantor Set Length Scales Illustration.png]]

Write 

$N_{\text{box}}(\epsilon)=N_a(\epsilon)+N_b(\epsilon)$

$N_{a}(\epsilon)=$ Number of boxes of size $\epsilon$ needed to cover $\lambda_{a}$
$N_{b}(\epsilon)=$ Number of boxes of size $\epsilon$ needed to cover $\lambda_{b}$

[[Self Similarity]] $\implies$ 

$N_{\text{box}}(\epsilon/{\lambda_a})=N_a(\epsilon)$
$N_{\text{box}}(\epsilon/{\lambda_b})=N_b(\epsilon)$

i.e. to cover strip $\lambda_a$ with boxes of size $\epsilon$ is like covering the full unit interval with boxes of size $\epsilon/{\lambda_a}$.

$D_0$ is definted as the scaling exponent $N_{\text{box}}=A\epsilon^{-D_0}$
$\implies$

$\underbrace{N_{\text{box}}(\epsilon)}_{A\epsilon^{-D_0}}=\underbrace{N_a(\epsilon)}_{N_{\text{box}}(\epsilon/{\lambda_a})}+\underbrace{N_b(\epsilon)}_{N_{\text{box}}(\epsilon/\lambda_b)}$

Here $\lambda_a=1/4$ and $\lambda_b=1/2$

$1=\left(\frac 14\right)^{D_0}+\left(\frac 12\right)^{D_0}=\left(\frac 1 {2^{D_0}}\right)^2+\frac{1}{2^{D_0}}$
(Quadratic equation in $x=(1/2)^{D_0}$)
$\frac{1}{2^{D_0}}=\frac{-1\pm \sqrt{5}}{2}$
$D_0=-\frac{\ln(\frac{-1+\sqrt 5}{2})}{\ln 2}\approx 0.69$

> Note: As a comparison, the naïve result is $\frac{\ln 3}{\ln 4}\approx 0.79$. Note that the symmetric case $\lambda_a=\lambda_b=\frac 13$ gives the middle-third result as before.
> $1=(1/3)^{D_0}+(1/3)^{D_0}=2(1/3)^{D_0}$
> $\implies D_0=\frac{\ln(1/2)}{\ln(1/3)}=\frac{\ln 2}{\ln 3}$