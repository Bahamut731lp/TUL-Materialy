> [!example] Vypočtěte
> $$\Large \int_0^{1} \frac{x^4}{\left(e^{x^5}\right)^5}\;dx$$

$$\large
\begin{align}
	&= \int_0^{1} \frac{x^4}{e^{5x^5}}\;dx \\
	&= \frac{1}{25}\int_0^{1} \frac{25x^4}{e^{5x^5}}\;dx
\end{align}
$$

> [!tip]- Substituce
>
>$$\large\begin{aligned}
u &= 5x^5 \\
du &= 25x^4 \\
>\end{aligned}$$

$$\large
\begin{align}
	&= \frac{1}{25}\int_0^{5} \frac{1}{e^{u}}\;du \\
	&= \frac{1}{25}\int_0^{5} e^{-u}\;du
\end{align}
$$

> [!tip]- Substituce
>
>$$\large\begin{aligned}
v &= -u \\
dv &= -du \\
>\end{aligned}$$

$$\large
\begin{align}
	&= -\frac{1}{25}\int_{0}^{-5} e^{v}\;dv \\
	&= \frac{1}{25}\int_{-5}^{0} e^{v}\;dv \\
\end{align}
$$

> [!warning] Pozor na hranice integrace
>Pro $a > b$ platí, že $\int_a^b f(x) = -\int_b^a f(x)$.
>viz [[Integrační meze#Otočení integračních mezí]]

$$\large
\begin{align}
	&= \frac{1}{25}\left[e^v\right]^{0}_{-5} \\
	&= \frac{1}{25}\cdot\left(e^0 - e^{-5}\right) \\
	&= \boxed{\frac{1}{25}\cdot\left(1 - e^{-5}\right)} \\
\end{align}
$$