> [!example] Vypočtěte
> $$\Large \int_{1}^{2} (x-2)\ln(4x)\;dx$$

> [!tip]+ Aplikace [[Per Partes#Metoda DI|DI metody]]
> Sestavíme si DI tabulku:
>
>||D | I |
|:---:|:----------------:|:-------------:|
|+|$\ln(4x)$ | $x-2$ |
|-|$\frac{4}{4x}$|$\frac{x^2}{2}-2x$|
>Zapíšeme výsledek: $\ln(4x)\cdot\left(\frac{x^2}{2}-2x\right) - \int_{1}^{2}\frac{4}{4x}\cdot\left(\frac{x^2}{2}-2x\right)$

$$\large
\begin{align}
	&= \left[\ln(4x)\cdot\left(\frac{x^2}{2}-2x\right)\right]_{1}^{2} - \int_{1}^{2}\frac{1}{\cancel{x}^1}\cdot\left(\frac{\cancel{x^2}^x}{2}-2\cancel{x}^1\right)\;dx \\
	&= \left[\ln(4x)\cdot\left(\frac{x^2}{2}-2x\right)\right]_{1}^{2} - \frac{1}{2}\int_{1}^{2}x\;dx + 2\int_{1}^{2}1\;dx \\
	&= \left[\ln(4x)\cdot\left(\frac{x^2}{2}-2x\right) - \frac{x^2}{4}\right]_{1}^{2} + 2\int_{1}^{2}1\;dx \\
	&= \left[\ln(4x)\cdot\left(\frac{x^2}{2}-2x\right) - \frac{1}{2}\cdot\frac{x^2}{2}\right]_{1}^{2} + 2\int_{1}^{2}1\;dx \\
	&= \left[\ln(4x)\cdot\left(\frac{x^2}{2}-2x\right) - \frac{x^2}{4} + 2x\right]_{1}^{2}\\
	&= \left[\ln(8)\cdot\left(\frac{4}{2}-4\right) - \frac{4}{4} + 4\right] - \left[\ln(4)\cdot\left(\frac{1}{2}-2\right) - \frac{1}{4} + 2\right]\\
	&= \left[-2\ln(8) + 3\right] - \left[-\frac{3}{2}\ln(4)-\frac{1}{4} + \frac{8}{4}\right]  \\
	&= -2\ln\left(2^3\right) + 3 + \frac{3}{2}\ln\left(2^2\right) - \frac{7}{4} \\
	&= -6\ln(2) + 3 + \frac{6}{2}\ln(2) - \frac{7}{4} \\
	&= -6\ln(2) + \frac{12}{4} + 3\ln(2) - \frac{7}{4} \\
	&= \boxed{-3\ln(2) + \frac{5}{4}}
\end{align}
$$

>[!info]
>$\log(a^c) = c\cdot\log(a)$