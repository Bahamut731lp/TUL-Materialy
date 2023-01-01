> [!example] Vypočtěte
> $$\Large \int_{-\frac{\pi}{2}}^{0} \frac{\sin(x)\cos(x)}{25 + 10\sin(x)+\sin^2(x)}\;dx$$

$$\large
\begin{align}
	&= \int_{-\frac{\pi}{2}}^{0} \frac{\sin(x)\cos(x)}{\left(\sin(x)+5\right)^2}\;dx
\end{align}
$$

> [!tip]+ Substituce
>
>$$\large\begin{aligned}
u &= 5 + \sin(x) \\
du &= \cos(x) \\
>\end{aligned}$$

$$\large
\begin{align}
	&= \int_4^{5} \frac{u-5}{u^2}\;du \\
	&= \int_4^{5} \frac{u}{u^2}\;du - \int_4^{5} \frac{5}{u^2}\;du \\
	&= \int_4^{5} \frac{1}{u}\;du - 5\int_4^{5} \frac{1}{u^2}\;du \\
	&= \left[\ln(u)\right]_{4}^{5} - 5\left[-\frac{1}{u}\right]_{4}^{5} \\
	&= \ln(5)-\ln(4)-5\left(-\frac{1}{5}+\frac{1}{4}\right) \\
	&= \ln\left(\frac{5}{4}\right) + 1 - \frac{5}{4} \\
	&= \boxed{\ln\left(\frac{5}{4}\right)- \frac{1}{4}} \\
\end{align}
$$