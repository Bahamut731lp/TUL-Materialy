> [!example] Vypočtěte
> $$\Large \int_{e}^{e^2} \frac{2+\ln{x}}{x\cdot(\ln^2{x} + 4\ln{x} + 4)}\;dx$$

> [!tip]+ Substituce
>
>$$\large\begin{aligned}
u &= \ln{x} \\
du &= \frac{1}{x} \\
>\end{aligned}$$

>[!info]
>$$\ln{(e)} = 1$$
>$$\ln{(a^b)} = b\cdot\ln{(a)}$$

$$
\begin{aligned}
	&= \int_{e}^{e^2} \frac{2+\ln{x}}{x\cdot(\ln^2{x} + 4\ln{x} + 4)}\;dx \\
	&= \int_{1}^{2} \frac{2+u}{u^2 + 4u + 4}\;du \\
	&= \int_{1}^{2} \frac{\cancel{u+2}}{\cancel{(u+2)}\cdot(u+2)}\;du \\
	&= \int_{1}^{2} \frac{1}{u+2} \;du \\
	&= \left[\ln|u+2|\right]_{1}^{2} \\
	&= \ln|4| - \ln|3| \\
	&= \boxed{\ln\left|\frac{4}{3}\right|}
\end{aligned}
$$

>[!info]
>$$\ln{a} - \ln{b} = \ln{\frac{a}{b}}$$
>viz [[Logaritmus]]