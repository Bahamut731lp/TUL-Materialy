> [!example] Vypočtěte
> $$\Large \int_{\ln{3}}^{\ln{5}} \frac{e^{3x}+e^{2x}}{e^{2x}-4e^x+4}\;dx$$

$$\large
\begin{align}
	&= \int_{\ln{3}}^{\ln{5}} \frac{e^x\cdot(e^{2x}+e^{x})}{e^{2x}-4e^x+4}\;dx \\
\end{align}
$$

> [!tip]+ Substituce
>
>$$\large\begin{aligned}
u &= e^x \\
du &= e^xdx \\
>\end{aligned}$$

$$\large
\begin{align}
	&= \int_{3}^{5} \frac{u^2+u}{u^2-4u+4}\;du \\
\end{align}
$$

> [!tip]+ Dělení polynomů
>
>$$\large\begin{aligned}
>(u^2+u) &: (u^2-4u+4) = 1 + \frac{5u-4}{u^2-4u+4}\\
>-(u^2-4u+4) \\
>\\
>5u-4 \\
>\end{aligned}$$

$$\large
\begin{align}
	&= \int_{3}^{5} 1+ \frac{5u-4}{u^2-4u+4}\;du \\
	&= \int_{3}^{5} 1\;du + \int_{3}^{5}\frac{5u-4}{u^2-4u+4}\;du \\
	&= \int_{3}^{5} 1\;du + \int_{3}^{5}\frac{5u-4}{u^2-4u+4}\;du \\
	&= \left[u\right]_{3}^{5} + 5\int_{3}^{5}\frac{u}{(u-2)^2}\;du - 4\int_{3}^{5}\frac{1}{(u-2)^2}\;du \\
\end{align}
$$

> [!tip]+ Substituce
>
>$$\large\begin{aligned}
v &= u-2 \\
dv &= du \\
>\end{aligned}$$

$$\large
\begin{align}
	&= \left[u\right]_{3}^{5} + 5\int_{1}^{3}\frac{v+2}{v^2}\;dv - 4\int_{1}^{3}\frac{1}{v^2}\;du \\
	&= \left[u\right]_{3}^{5} + 5\int_{1}^{3}\frac{v}{v^2}\;dv + 10\int_{1}^{3}\frac{1}{v^2}\;dv - 4\int_{1}^{3}\frac{1}{v^2}\;du \\
	&= \left[u\right]_{3}^{5} + 5\int_{1}^{3}\frac{1}{v}\;dv + 6\int_{1}^{3}\frac{1}{v^2}\;dv\\
	&= \left[u\right]_{3}^{5} + 5\left[\;\ln|u|\;\right]_{1}^{3} + 6\left[\;-\frac{1}{v}\;\right]_{1}^{3}\\
	&= 2 + 5[\ln(3)-\ln(1)] + 6\left[\;-\frac{1}{3} + 1\;\right]_{1}^{3}\\
	&= 2 + 5\ln(3) + -2 + 6\\
	&= \boxed{6 + 5\ln(3)}\\
\end{align}
$$