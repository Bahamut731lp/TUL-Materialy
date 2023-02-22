> [!example] Spočtěte obsah obrazce
> ohraničeného funkcemi $\cos{(\frac{\pi{x}}{2})}$ a $x^2-1$

>[!info]
>$$\begin{aligned}
>f(x) &= \cos{(\frac{\pi{x}}{2})} \\
>g(x) &= x^2-1
>\end{aligned}$$

>[!info] Vypočítání [[Integrační meze]]
>$f(x) = 0, x = 1, -1, 3, -3, ...$
>$g(x) = 0, x = 1, -1$
>- Integrál budeme počítat na intervalu $\left<-1, 1\right>$
>- Monotonie funkce $f(x)$
![[priklad_46_funkce_f.png]]
>- Monotonie funkce $g(x)$
>![[priklad_46_funkce_g.png]]
$$
\begin{aligned}
	&= \int_{-1}^{1} f(x) - g(x)\;dx \\
	&= \int_{-1}^{1} \cos{\left(\frac{\pi{x}}{2}\right)}\;dx - \int_{-1}^{1}x^2\;dx+\int_{-1}^{1}1\;dx \\
\end{aligned}
$$

> [!tip]+ Substituce
>
>$$\large\begin{aligned}
u &= \frac{\pi}{2}{x} \\
du &= \frac{\pi}{2} \\
>\end{aligned}$$

$$
\begin{aligned}
	&= \int_{-1}^{1} \cos{\left(\frac{\pi{x}}{2}\right)}\;dx - \int_{-1}^{1}x^2\;dx+\int_{-1}^{1}1\;dx \\
	&= \frac{2}{\pi}\int_{-1}^{1} \cos{\left(\frac{\pi{x}}{2}\right)}\;dx - \int_{-1}^{1}x^2\;dx+\int_{-1}^{1}1\;dx \\
	&= \frac{2}{\pi}\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}} \cos{(u)}\;dx - \left[\frac{x^3}{3}\right]_{-1}^{1}+\left[x\right]_{-1}^{1} \\
	&= \frac{2}{\pi}\left[\sin(u)\right]_{-\frac{\pi}{2}}^{\frac{\pi}{2}} - \left[\frac{x^3}{3}\right]_{-1}^{1}+\left[x\right]_{-1}^{1} \\
	&= \frac{2}{\pi}\left[1 + 1\right] - \frac{2}{3} + 2 \\
	&= \frac{4}{\pi}-\frac{2}{3}+2 \\
	&= \boxed{\frac{4}{\pi}+\frac{4}{3}}
\end{aligned}
$$