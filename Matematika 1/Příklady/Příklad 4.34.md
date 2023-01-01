> [!example] Vypočtěte
> $$\Large \int_{0}^{\ln(2)} \frac{5e^x}{15+8e^x+e^{2x}}\;dx$$

> [!tip]+ Substituce
>
>$$\large\begin{aligned}
u &= e^x \\
du &= e^x\;dx \\
>\end{aligned}$$

$$\large
\begin{align}
	&= 5\int_{1}^{2} \frac{1}{15+8u+u^{2}}\;du \\
	&= 5\int_{1}^{2} \frac{1}{(u+5)(u+3)}\;du \\
\end{align}
$$

> [!tip]+ Rozklad na [[Rozklad na parciální zlomky|parciální zlomky]]
>
>$$\large\begin{aligned}
\frac{A}{(u+5)} + \frac{B}{(u+3)} = \begin{cases}
A = -\frac{1}{2} \\
B = \frac{1}{2}
\end{cases} \\
>\end{aligned}$$

$$\large
\begin{align}
	&= 5\int_{1}^{2} -\frac{1}{2}\frac{1}{u+5} + \frac{1}{2}\frac{1}{u+3}\;du \\
	&= -\frac{5}{2}\int_{1}^{2}\frac{1}{u+5} + \frac{5}{2}\int_{1}^{2}\frac{1}{u+3}\;du \\
	&= -\frac{5}{2}\left[\ln(u+5)\right]_{1}^{2} + \frac{5}{2} \left[\ln(u+3)\right]_{1}^{2} \\
	&= -\frac{5}{2}\left[\ln(7) - \ln(6)\right] + \frac{5}{2} \left[\ln(5) - \ln(4)\right] \\
	&= -\frac{5}{2}\left[\ln\left(\frac{7}{6}\right)\right] + \frac{5}{2} \left[\ln\left(\frac{5}{4}\right)\right] \\
	&= \frac{5}{2}\left(\ln\left(\frac{5}{4}\right) - \ln\left(\frac{7}{6}\right)\right) \\
	&= \frac{5}{2}\left(\ln\left(\frac{5}{\cancel{4}^2}\cdot\frac{\cancel{6}^3}{7}\right)\right) \\
	&= \frac{5}{2}\left(\ln\left(\frac{5}{2}\cdot\frac{3}{7}\right)\right) \\
	&= \boxed{\frac{5}{2}\left(\ln\left(\frac{15}{14}\right)\right)} \\
\end{align}
$$