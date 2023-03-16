> [!example] Vypočtěte
> $$\Large \int_{0}^{1} \frac{2-3\arcsin(x)}{\sqrt{1-x^2}}\;dx$$

$$
\begin{aligned}
	&\int_{0}^{1} \frac{2-3\arcsin(x)}{\sqrt{1-x^2}}\;dx \\
	&= \int_{0}^{1} \frac{2}{\sqrt{1-x^2}}\;dx - \int_{0}^{1} \frac{3\arcsin(x)}{\sqrt{1-x^2}}\;dx \\
	&= 2\int_{0}^{1} \frac{1}{\sqrt{1-x^2}}\;dx - 3\int_{0}^{1} \frac{\arcsin(x)}{\sqrt{1-x^2}}\;dx
\end{aligned}
$$

> [!tip]+ Substituce
>
>$$\large\begin{aligned}
u &= \arcsin(x) \\
du &= \frac{1}{\sqrt{1-x^2}}dx \\
>\end{aligned}$$

>[!info]
>$$\arcsin(0) = 0$$
>$$\arcsin(1) = \frac{\pi}{2}$$

$$
\begin{aligned}
	&= 2\int_{0}^{1} \frac{1}{\sqrt{1-x^2}}\;dx - 3\int_{0}^{1} \frac{\arcsin(x)}{\sqrt{1-x^2}}\;dx \\
	&= 2\int_{0}^{\frac{\pi}{2}}\;du - 3\int_{0}^{\frac{\pi}{2}} u\;du \\
	&= 2\cdot\left[u\right]_{0}^{\frac{\pi}{2}} - 3\cdot\left[\frac{u^2}{2}\right]_{0}^{\frac{\pi}{2}} \\
	&= \cancel{2}\frac{\pi}{\cancel{2}} - 3\cdot\left[\frac{\left(\frac{\pi}{2}\right)^2}{2} - \frac{0}{2}\right] \\
	&= \pi -3 \cdot \left[\frac{\pi^2}{4}\cdot\frac{1}{2}\right] \\
	&= \boxed{\pi - \frac{3\pi^2}{8}} \\
\end{aligned}
$$

