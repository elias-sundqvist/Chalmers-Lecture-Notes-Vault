The quantity $S=-\sum_kp_k(\epsilon)\ln p_k(\epsilon)=-\left<\ln p(\epsilon) \right>$ is the *Shannon Entropy*. 

Given an experiment with $r$ possible outcomes, with probabilities $p_1,p_2,\dots,p_r$, $\sum_{k=1}^rp_k=1$, the Shannon entropy is

$S=-\sum_{k=1}^r p_k\ln p_k$

with $p_k\ln p_k=0$ if $p_k=0$

#### Simlest Case

$p_i=1$ if $k=i$ and $0$ otherwise $\implies S=0$

#### Case Of Maximum Uncertainty
$p_k=1/r\implies S=\ln r$

In general $0\le S\le \ln r$, the closer $S$ is to $\ln r$ the more uncertain the outcome of an experiment is. For the [[Information Dimension]]: $r=N_{\text{box}}$ and $S$ quantifies tha amount of (Shannon) information needed to describe the content of the boxes for a given accuracy $\epsilon$. The information dimension tells how this amount of information scales with the resolution $\epsilon$, $S(\epsilon)\sim -D_1\ln \epsilon$