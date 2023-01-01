> [!example] Vypočtěte
> $$\Large \int_{0}^{\pi} \frac{\sin(x)\cdot(5-3\cos(x)+\cos^2(x))}{4-4\cos(x)+\cos^2(x)}\;dx$$

$$\large
\begin{align}
	&= -\int_{0}^{\pi} \frac{-\sin(x)\cdot(5-3\cos(x)+\cos^2(x))}{4-4\cos(x)+\cos^2(x)}\;dx \\
\end{align}
$$

> [!tip]+ Substituce
>$$\large\begin{aligned}
u &= cos(x) \\
du &= -sin(x)dx \\
>\end{aligned}$$

$$\large
\begin{align}
	&= -\int_{1}^{-1} \frac{u^2-3u+5}{u^2-4u+4}\;du \\
\end{align}
$$

>[!warning] Pozor na prohození integračních mezí
>viz [[Integrační meze#Otočení integračních mezí]]

$$\large
\begin{align}
	&= \int_{-1}^{1} \frac{u^2-3u+5}{u^2-4u+4}\;du \\
\end{align}
$$

> [!tip]+ Dělení polynomů
>
>$$\large\begin{aligned}
>(u^2-3u+5) &: (u^2-4u+4) = 1 + \frac{u+1}{u^2-4u+4}\\
>-(u^2-4u+4) \\
>\\
>u+1 \\
>\end{aligned}$$

$$\large
\begin{align}
	&= \int_{-1}^{1} 1 + \frac{u+1}{u^2-4u+4}\;du \\
	&= \int_{-1}^{1} 1\;du + \int_{-1}^{1}\frac{u+1}{(u-2)^2}\;du \\
	&= \left[u\right]_{-1}^{1} + \int_{-1}^{1}\frac{u}{(u-2)^2}\;du +\int_{-1}^{1}\frac{1}{(u-2)^2}\;du \\
\end{align}
$$

> [!tip]+ Substituce
>$$\large\begin{aligned}
v &= u - 2 \\
dv &= du \\
>\end{aligned}$$

$$\large
\begin{align}
	&= \left[u\right]_{-1}^{1} + \int_{-3}^{-1}\frac{v+2}{v^2}\;dv +\int_{-3}^{-1}\frac{1}{v^2}\;dv \\
	&= 2 + \int_{-3}^{-1}\frac{v}{v^2}\;dv + \int_{-3}^{-1}\frac{2}{v^2}\;dv +\int_{-3}^{-1}\frac{1}{v^2}\;dv \\
	&= 2 + \int_{-3}^{-1}\frac{1}{v}\;dv + 2\int_{-3}^{-1}\frac{1}{v^2}\;dv +\int_{-3}^{-1}\frac{1}{v^2}\;dv \\
	&= 2 + \int_{-3}^{-1}\frac{1}{v}\;dv + 3\int_{-3}^{-1}\frac{1}{v^2}\;dv \\
	&= 2 + \left[\ln|v|\right]_{-3}^{-1} + 3\left[-\frac{1}{v}\right]_{-3}^{-1} \\
	&= 2 + \left(\ln(1) - \ln(3)\right) + 3\left[1 -\frac{1}{3}\right]_{-3}^{-1} \\
	&= 2 - \ln(3) + 3 - 1 \\
	&= \boxed{4 - \ln(3)} \\
\end{align}
$$