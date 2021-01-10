To find an analytical expression for the [[Lyapunov Exponent|Lyapunov exponents]]

First write $\mathbb M =\mathbb M \mathbb I$, with the [[Unit Matrix|unit matrix]] $\mathbb I=[\hat{\mathbf e}^{(1)}\hat{\mathbf e}^{(2)}\dots\hat{\mathbf e}^{(n)}]$, using a cartesian coordinate system $\hat{\mathbf e}^{(i)}$ with elements $e_j^{(i)}=\delta_{i,j}$, where $i,j\in 1,\dots,n$.

The first $K$ of these basis vectors span a $K$-dimensional hypercube with unit volume. Ler $\mathbf m^{(i)}$ be column vectors in the deformation  matrix, $\mathbb M=[\mathbf m^{(1)}\mathbf m^{(2)}\dots \mathbf m^{(n)}]$, let $\mathbf 0$ be the column vector of zeroes, and use $\mathbb M$ to deform a hypercube with small volumne $\mathcal V_{K,0}$:

$\mathbb M[\hat{\mathbf e}^{(1)}\hat{\mathbf e}^{(2)}\dots\hat{\mathbf e}^{(K)}\mathbf 0\dots \mathbf 0]\mathcal V_{K,0}$

The column vectors of the resulting matrix, $\mathbf m^{(\alpha)}$ with $\alpha=1,\dots,K$. span a $K$-dimensional hyperparallelepiped (embedded in $n$ dimensions). Its volume $\mathcal V_K=\sqrt{|\det \mathbb G^{(K)}|}\mathcal V_{K,0}$, where $\mathbb G^{(K)}$ is the [[Gram Matrix]] of the spanning vectors with elements $\mathbb G_{\alpha\beta}^{(K)}=\mathbb m^{\alpha}\cdot \mathbb m^{(\beta)}$, with $\alpha, \beta=1,\dots,K$.

Now, factorize $\mathbb M$ using [[QR-Decomposition]], $\mathbb M=\mathbb Q\mathbb R$, to obtain.

$\mathbb G_{\alpha\beta}^{(K)}=[\mathbb m^{(\alpha)}]^T\mathbb m^{(\beta)}=[\mathbb M^T\mathbb M]_{\alpha\beta}=[\mathbb R^T\mathbb Q^T\mathbb Q\mathbb R]_{\alpha\beta}=[\mathbb R^T\mathbb R]_{\alpha\beta}$ where $\alpha,\beta=1,\dots,K$.

Using that the determinant of a right triangular matrix $\mathbb R$ is equal to the product of the diagonal elements gives

$\frac{\mathcal V_K}{\mathcal V_{K,0}}=\sqrt{|\det{\mathbb F^{(K)}}|}=\sqrt{|\det(\mathbb R_K^T\mathbb R_K)|}=|\det \mathbb R_K|=\prod_{\alpha=1}^K|\mathbb R_{\alpha\alpha}|$

where $\mathbb R_K$ is the first $K\times K$ matrix in $\mathbb R:$

$\mathbb R_K\equiv\begin{pmatrix}\mathbb R_{11}&\mathbb R_{12}&\dots&\mathbb R_{1K}\\0&\mathbb R_{22}&\ddots&\vdots\\\vdots&\ddots&\ddots&\mathbb R_{K-1,K}\\0&\dots&0&\mathbb R_{KK}\end{pmatrix}$

Inserting into the definition of the [[Lyapunov Spectrum]] gives

$\lambda_1+\dots+\lambda_K=\underset{t\rightarrow\infty}{\lim}\;\frac 1 t\ln\left(\prod_{\alpha=1}^K|\mathbb R_{\alpha\alpha}|\right)=\sum_{\alpha=1}^K\underset{t\rightarrow \infty}{\lim}\;\frac 1t\ln(|\mathbb R_{\alpha\alpha}|)$

By inserting $K=1$, $K=2$, $\dots$, $K=n$ in this relation, it follows that the ordered Lyapunov exponents are given by the diagonal elements of $\mathbb R$:

$\lambda_i=\underset{t\rightarrow\infty}{\lim}\;\frac 1t \ln|\mathbb R_{ii}|$

This relation is useful for [[Numerical Computation Of Deformation Matrix|evaluating Lyapunov exponents numerically]].  The lyapunov exponents are real numbers. Due to the singular nature of $\mathbb M$ at large $t$, we generically have $\lambda_i=\text{Re}\overset \sim \sigma_i$, but counterexamples can be constructed.

The [[Lyapunov Exponent|Lyapunov exponents]] (and [[Stability Exponents Of Trajectory Separations|stability exponents of separations]]) are useful to understand the behaviour of regular and [[Chaotic Systems|chaotic systems]]s. Their signs quantify the attractors of a system, and their relative magnitudes give information on the degree of fractal clustering in [[Chaotic Systems|chaotic systems]]. 