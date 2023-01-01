> [!example] Vypočtěte
> $$\Large \int_{0}^{1} \frac{1}{\sqrt{1-x^2}\sqrt[3]{\arccos(x)}}\;dx$$

$$\large
\begin{align}
	&= -\int_{0}^{1} -\frac{1}{\sqrt{1-x^2}}\cdot\frac{1}{\sqrt[3]{\arccos(x)}}\;dx \\
\end{align}
$$

> [!tip]+ Substituce
>
>$$\large\begin{aligned}
u &= \arccos(x) \\
du &= -\frac{1}{\sqrt{1-x^2}}dx \\
>\end{aligned}$$

$$\large
\begin{align}
	&= -\int_{\frac{\pi}{2}}^{0} \frac{1}{\sqrt[3]{u}}\;du \\
\end{align}
$$

>[!warning] Pozor na prohození integračních mezí
>viz [[Integrační meze#Otočení integračních mezí]]

$$\large
\begin{align}
	&= \int_{0}^{\frac{\pi}{2}} \frac{1}{\sqrt[3]{u}}\;du \\
	&= \int_{0}^{\frac{\pi}{2}} u^{-\frac{1}{3}}\;du \\
	&= \left[ \frac{u^{\frac{2}{3}}}{\frac{2}{3}}\right]_{0}^{\frac{\pi}{2}} \\
	&= \left[ \frac{3}{2}\sqrt[3]{u^2}\right]_{0}^{\frac{\pi}{2}} \\
	&= \left[ \frac{3}{2}\sqrt[3]{\left(\frac{\pi}{2}\right)^2}\right] - \left[ \frac{3}{2}\sqrt[3]{0^2}\right]\\
	&= \left[ \frac{3}{2}\sqrt[3]{\frac{\pi^2}{4}}\right] - 0\\
	&= \boxed{\frac{3}{2}\sqrt[3]{\frac{\pi^2}{4}}}
\end{align}
$$