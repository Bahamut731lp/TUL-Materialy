# Bernoulliho diferenciální rovnice
Bernoulliho diferenciální rovnice (BDR) jsou rovnice ve tvaru:
>$$\Large\begin{aligned}y'+f(x)y&=g(x)y^n \\n&\in\mathbb{R}\setminus\set{0, 1} \\
\end{aligned}$$

BDR řešíme převedením na LDR takto:

$$\large\begin{aligned}
\frac{y'}{y^n}+\frac{f(x)y^1}{y^n}&=g(x) \\
\frac{y'}{y^n}+f(x)y^{1-n}&=g(x) \\ \\
u&=y^{1-n} \\
u'&=(1 - n) \cdot y^{-n} \cdot y' \\
\end{aligned}$$