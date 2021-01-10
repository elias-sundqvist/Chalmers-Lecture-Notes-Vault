### The [[Analytical Analysis|analytic]] solutions to [[Linear 2D Flows]]

#### Solution for diagonalizable flows
In matrix form, we get 

$\dot{\mathbf x} = \mathbb A \mathbf x,\;\mathbb A=\begin{bmatrix}a&b\\c&d\end{bmatrix}$.
Assume $\mathbb A$ is diagonalizable, $\mathbb A=\mathbb P\mathbb D\mathbb P^{-1}$ with eigenvalue matrix.

$\mathbb D=\begin{bmatrix}\lambda_1&0\\0&\lambda_2\end{bmatrix}$

and $\mathbb P$ is a matrix spanned by the eigenvectors of $\mathbb A$. Then we can rewrite the equation as. 
$\dot{\mathbf x}=\mathbb P\mathbb D\mathbb P^{-1}x$
$\implies \frac{d}{dt}[\mathbb P^{-1}x]=\mathbb D\underbrace{\mathbb P^{-1} \mathbf x}_{\mathbf \xi}$
$\implies \dot{\mathbf \xi}=\mathbb D\mathbf \xi$
$\implies \mathbf \xi(t)=(e^{\lambda_1 t}\xi_1(0),e^{\lambda_2 t}\xi_2(0))$

For the case of complex eigenvalues $\lambda=\mu\mp i\omega$ with corresponding eigenvectors $\mathbf v$ and $\bar{\mathbf v}$, this solution becomes complex. Then choose 
$\mathbb D=\begin{bmatrix}\mu&-\omega\\\omega&\mu\end{bmatrix},\; \mathbb P=\begin{bmatrix}\text{Re}\left[v_1\right]&\text{Im}\left[v_1\right]\\\text{Re}\left[v_2\right]&\text{Im}\left[v_2\right]\end{bmatrix}$

such that $\mathbf \xi$ is real and $\dot {\mathbf \xi} =\mathbb D\mathbf \xi$, with solution (let $\xi_2(0)=0$)
$\mathbb \xi(t)=\xi_1(0)e^{\mu t}(\cos(\omega t),\sin(\omega t))$

So  the solution of diagonalizable matrices can be written on the form $\mathbb \xi (t)=\begin{bmatrix}e^{\lambda_1t}&0\\0&e^{\lambda_2 t}\end{bmatrix}\mathbb \xi(0)$

under a suitable choice of basis. 


#### Solution for non-diagonalizable flows
The non-diagonalizable case has a special solution $\dot{\mathbf \xi}=\begin{bmatrix}\lambda&1\\0&\lambda\end{bmatrix}\mathbf \xi\implies \mathbf \xi (t)=\exp\left[\begin{bmatrix}\lambda&1\\0&\lambda\end{bmatrix}t\right]\mathbf \xi(0)=\sum_{i=0}^{\infty}\frac{1}{i!}\left[\begin{bmatrix}\lambda&1\\0&\lambda\end{bmatrix} t\right]^i\mathbf \xi(0)=\dots$
where the sum can be evaluated by brute force. A more elegant solution is to write. 
$\begin{bmatrix}\lambda&1\\0&\lambda\end{bmatrix}=\mathbb B+ \mathbb C$ with $\mathbb B =\begin{bmatrix}\lambda&0\\0&\lambda\end{bmatrix}$, $\mathbb C=\begin{bmatrix}0&1\\0&0\end{bmatrix}$ and use that $\mathbb B$ and $\mathbb C$ commute because $\mathbb B$ is a multiple of the unit matrix:
> **Short Proof That $\mathbb B$ and $\mathbb C$ commute**
> $[\mathbb B,\mathbb C]=\mathbb B\mathbb C-\mathbb C\mathbb B=\lambda\mathbb I\mathbb C-\lambda\mathbb C\mathbb I=\lambda(\mathbb C-\mathbb C)=0$.

For commuting matrices we have $e^{\mathbb B}e^{\mathbb C}=e^{\mathbb B}+\mathbb C\implies$
$\mathbf \xi(t)=\exp\left[\begin{bmatrix}\lambda&0\\0&\lambda\end{bmatrix} t+ \begin{bmatrix}0&1\\0&0\end{bmatrix} t\right]\mathbb \xi (0)$
$=\exp\left[\begin{bmatrix}\lambda&0\\0&\lambda\end{bmatrix} t\right]\exp\left[\begin{bmatrix}0&1\\0&0\end{bmatrix} t\right]\mathbb \xi (0)$
$=e^{\lambda t}\begin{bmatrix}1&t\\0&1\end{bmatrix}\mathbb \xi(0)$
where in the last step we used that 

$\begin{bmatrix}0&t\\0&0\end{bmatrix}^i=\cases{\begin{bmatrix}1&0\\0&1\end{bmatrix}& if \(i=0\)\\\begin{bmatrix}0&t\\0&0\end{bmatrix}& if \(i=1\)\\\begin{bmatrix}0&0\\0&0\end{bmatrix}& if \(i=2,3,\dots\)}$

So the solution for non-diagonalizable matrices can be written on the form 
$\mathbf\xi(t)=e^{\lambda t}\begin{bmatrix}1&t\\0&1\end{bmatrix}$ under a suitable choice of basis. 