> [!example] Vypočtěte
> $$\Large \int_{1}^{e} 4x\cdot\ln(2x)\;dx$$

$$\large
\begin{align}
	&= \int_{1}^{e} 2x\cdot\ln(2x)\;2dx \\
\end{align}
$$

> [!tip]+ Substituce
>
>$$\large\begin{aligned}
u &= 2x \\
du &= 2dx \\
>\end{aligned}$$

$$\large
\begin{align}
	&= \int_{2}^{2e} u\cdot\ln(u)\;du \\
\end{align}
$$

> [!tip]+ Aplikace [[Per Partes#Metoda DI|DI metody]]
> Sestavíme si DI tabulku:
>
>||D | I 
|:---:|:----------------:|:-------------:|
|+|$\ln(u)$ | $u$ |
|-|$\frac{1}{u}$|$\frac{u^2}{2}$|
>Zapíšeme výsledek: $\frac{1}{2}\ln(u)u^2-\int_2^{2e}\frac{u}{2}\;du$

$$\large
\begin{align}
	&= \left[\frac{1}{2}\ln(u)u^2\right]_{2}^{2e}-\frac{1}{2}\int_2^{2e}u\;du \\
	&= \left[\frac{1}{2}\ln(u)u^2\right]_{2}^{2e}-\frac{1}{2}\left[\frac{u^2}{2}\right]_{2}^{2e} \\
	&= \frac{1}{2}\left(4e^2\ln(2e) - 4\ln(2)\right)-\frac{1}{2}\left[\frac{4e^2 - 4}{2}\right] \\
	&= \frac{1}{2}\left(4e^2\ln(2e) - 4\ln(2)\right)-\frac{1}{2}\left[{2e^2 - 2}\right] \\
	&= \left(2e^2(\ln(2) + \ln(e)) - 2\ln(2)\right)-e^2 + 1 \\
	&= 2e^2\ln(2) + 2e^2 - 2\ln(2)-e^2 + 1 \\
	&= 2e^2\ln(2) - 2\ln(2) + 1 + e^2 \\
	&= \boxed{\ln(2)\cdot(2e^2 - 2) + e^2 + 1} 
\end{align}
$$