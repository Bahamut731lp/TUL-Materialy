> [!example] Vypočtěte
> $$\Large \int_{0}^{\frac{\sqrt{2}}{2}} \frac{1}{\sqrt{1-x^2}\cdot\arccos(x)}\;dx$$

> [!tip]+ Substituce
>
>$$\large\begin{aligned}
u &= \arccos(x) \\
du &= -\frac{1}{\sqrt{1-x^2}}\;dx \\
>\end{aligned}$$

$$\large
\begin{align}
	&= -\int_{0}^{\frac{\sqrt{2}}{2}} -\frac{1}{\sqrt{1-x^2}}\cdot\frac{1}{\arccos(x)} \;dx \\
	&= -\int_{\frac{\pi}{2}}^{\frac{\pi}{4}} \frac{1}{u}\;du \\
\end{align}
$$

>[!warning] Pozor na prohození integračních mezí
>viz [[Integrační meze#Otočení integračních mezí]]

$$\large
\begin{align}
	&= \int_{\frac{\pi}{4}}^{\frac{\pi}{2}} \frac{1}{u}\;du \\
	&= \left[\;\ln|u|\;\right]_{\frac{\pi}{4}}^{\frac{\pi}{2}} \\
	&= \left[\ln\left|\frac{\pi}{2}\right| - \ln\left|\frac{\pi}{4}\right| \right] \\
	&= \ln\left|\frac{\cancel{\pi}^1}{\cancel{2}^1}\cdot\frac{\cancel{4}^2}{\cancel{\pi}^1}\right| \\
	&= \boxed{\ln(2)}
\end{align}
$$