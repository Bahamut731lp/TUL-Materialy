> [!example] Vypočtěte
> $$\Large \int_{-\infty}^{0} \frac{e^{2x}}{1+4e^{4x}}\;dx$$

> [!tip]+ Substituce
>
>$$\large\begin{aligned}
u &= e^x \\
du &= e^x\;dx \\
>\end{aligned}$$

$$\large
\begin{align}
	&= \int_{-\infty}^{0} \frac{e^{x} \cdot e^{x}}{1+4e^{4x}}\;dx \\
	&= \int_{0}^{1} \frac{u}{1+4u^4}\;du \\
\end{align}
$$

> [!tip]+ Substituce
>
>$$\large\begin{aligned}
v &= u^2 \\
dv &= 2u\;du \\
>\end{aligned}$$

$$\large
\begin{align}
	&= \frac{1}{2}\int_{0}^{1} \frac{2u}{1+4u^4}\;du \\
	&= \frac{1}{2}\int_{0}^{1} \frac{1}{1+4v^2}\;dv \\
	&= \frac{1}{2}\int_{0}^{1} \frac{1}{1+(2v)^2}\;dv \\
	&= \frac{1}{2}\int_{0}^{1} \frac{1}{1+(2v)^2}\;dv \\
\end{align}
$$

> [!tip]+ Substituce
>
>$$\large\begin{aligned}
t &= 2v \\
dt &= 2v\;du \\
>\end{aligned}$$

$$\large
\begin{align}
	&= \frac{1}{4}\int_{0}^{1} \frac{2}{1+(2v)^2}\;dv \\
	&= \frac{1}{4}\int_{0}^{2} \frac{1}{1+t^2}\;dv \\
	&= \frac{1}{4}\left[\arctan(t)\right]_{0}^{2} \\
	&= \boxed{\frac{1}{4}\arctan(2)} \\
\end{align}
$$