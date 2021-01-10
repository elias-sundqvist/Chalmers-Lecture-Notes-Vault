In [[Frictionless Mechanics]] we have the [[Hamiltonian Systems|hamiltonian]]

$H\equiv \frac{p^2}{2m}+V(x)$

By [[2D Linear Stability Analysis|linearizing]], we get 

$\mathbb J=\begin{bmatrix}\frac{\partial^2H}{\partial x\partial p}&\frac{\partial^2H}{\partial p^2}\\-\frac{\partial^2H}{\partial x^2}&-\frac{\partial^2H}{\partial p\partial x}\end{bmatrix}=\begin{bmatrix}0&\frac 1 m\\-\frac{\partial^2V}{\partial x^2}&0\end{bmatrix}$

At any fixed point we have $\tau \equiv \text{Tr}\mathbb J=0$ and $\Delta\equiv \det\mathbb J(\mathbf x^*)=V''(\mathbf x^*)/m$, i.e. $\lambda_{1,2}=\pm \sqrt{-\det \mathbb J}$

If $V''(\mathbf x^*)<0$ then $\lambda_{1,2}=\pm \sqrt{|V''(\mathbf x^*)|/m}$ ([[Saddle Point|Saddle]])
If $V''(\mathbf x^*)>0$ then $\lambda_{1,2}=\pm i\sqrt{|V''(\mathbf x^*)|/m}$ ([[Center|Center]])

[[Fixed Points|Fixed points]] are located at $\dot x = p=0$ and $\dot p =-V'(x)=0\implies$ Centers at [[Potential Minimum|potential minima]] and saddles at [[Potential Maximum|potential maxima]]. 