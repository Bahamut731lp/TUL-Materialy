> [!example] Vypočtěte
> $$\Large \int_{0}^{2} \frac{-4x}{4+x^2}\;dx$$

$$\large
\begin{align}
	&= -2\int_{0}^{2} \frac{2x}{4+x^2}\;dx \\
\end{align}
$$

> [!tip]+ Substituce
>
>$$\large\begin{aligned}
u &= x^2 \\
du &= 2xdx \\
>\end{aligned}$$

$$\large
\begin{align}
	&= -2\int_{0}^{4} \frac{1}{u+4}\;du \\
	&= -2\left[\ln\left|u+4\right|\right]_{0}^{4} \\
	&= -2\left(\ln\left|8\right| - \ln\left|4\right|\right)\\
	&= -2\left(\ln\left|\frac{\cancel{8}^2}{\cancel{4}^1}\right|\right)\\
	&= \boxed{-2\ln\left|2\right|}\\
\end{align}
$$