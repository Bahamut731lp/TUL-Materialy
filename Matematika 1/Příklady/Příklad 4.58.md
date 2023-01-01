> [!example] Vypočtěte
> $$\Large \int_{0}^{1} 8x\cdot\arctan(2x)\;dx$$

$$\large
\begin{align}
	&= \int_{0}^{1} 4x\cdot\arctan(2x)\;2dx \\
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
	&= \int_{0}^{2} 2u\cdot\arctan(u)\;2du \\
	&= 2\int_{0}^{2} u\cdot\arctan(u)\;2du \\
\end{align}
$$

> [!tip]+ Aplikace [[Per Partes#Metoda DI|DI metody]]
> Sestavíme si DI tabulku:
>
>||D | I 
|:---:|:----------------:|:-------------:|
|+|$\arctan(u)$ | $u$ |
|-|$\frac{1}{u^2+1}$|$\frac{u^2}{2}$|
>Zapíšeme výsledek: $\arctan(u)\cdot\frac{u^2}{2}-\int_0^{2}\frac{1}{u^2+1}\cdot\frac{u^2}{2}\;du$

$$\large
\begin{align}
	&= 2\left[\arctan(u)\cdot\frac{u^2}{2}\right]_{0}^{2}-2\int_0^{2}\frac{1}{u^2+1}\cdot\frac{u^2}{2}\;du \\
	&= \left[\arctan(u)\cdot{u^2}\right]_{0}^{2}-\int_0^{2}\frac{u^2}{u^2+1}\;du \\
\end{align}
$$

> [!tip]+ Dělení polynomů
>
>$$\large\begin{aligned}
>(u^2) &: (u^2+1) = 1 - \frac{1}{u^2 + 1}\\
>-(u^2+1) \\
>\\
>-1\\
>\end{aligned}$$

$$\large
\begin{align}
	&= \left[\arctan(u)\cdot{u^2}\right]_{0}^{2}-\int_0^{2}1 - \frac{1}{u^2 + 1}\;du \\
	&= \left[\arctan(u)\cdot{u^2}\right]_{0}^{2}-\int_0^{2}1\;du + \int_0^{2}\frac{1}{u^2 + 1}\;du \\
	&= \left[\arctan(u)\cdot{u^2} - u\right]_{0}^{2} + \int_0^{2}\frac{1}{u^2 + 1}\;du \\
	&= \left[\arctan(u)\cdot{u^2} - u + \arctan(u)\right]_{0}^{2} \\
\end{align}
$$

>[!info]
>$\arctan(0) = 0$

$$\large
\begin{align}
	&= \left[4\arctan(2) - 2 + \arctan(2)\right] - \left[0\arctan(0) - 0 + \arctan(0)\right]\\
	&= 4\arctan(2) - 2 + \arctan(2)\\
	&= \boxed{5\arctan(2) - 2}\\
\end{align}
$$

