> [!example] Vypočtěte
> $$\Large \int_{1}^{e} \frac{\ln(x)}{x\cdot(1+2\ln(x)+\ln^2(x))}\;dx$$

> [!tip]+ Substituce
>
>$$\large\begin{aligned}
u &= \ln(x) \\
du &= \frac{1}{x}dx \\
>\end{aligned}$$

$$\large
\begin{align}
	&= \int_{0}^{1} \frac{u}{1+2u+u^2}\;du \\
	&= \int_{0}^{1} \frac{u}{(u+1)^2}\;du \\
\end{align}
$$

> [!tip]+ Substituce
>
>$$\large\begin{aligned}
v &= u+1 \\
dv &= du \\
>\end{aligned}$$

$$\large
\begin{align}
	&= \int_{1}^{2} \frac{v-1}{v^2}\;dv \\
	&= \int_{1}^{2} \frac{\cancel{v}^1}{\cancel{v^2}^v}\;dv - \int_{1}^{2} \frac{1}{v^2}\;dv \\
	&= \int_{1}^{2} \frac{1}{v}\;dv - \int_{1}^{2} v^{-2}\;dv \\
	&= \left[\;\ln|v|\;\right]_{1}^{2} - \left[\;\ln\left|-\frac{1}{v}\right|\;\right]_{1}^{2} \\
	&= \left(\;\ln|2| - \ln|1| \;\right) - \left(\;-\frac{1}{2} + 1\right) \\
	&= \ln|2| + \frac{1}{2} - 1 \\
	&= \boxed{\ln|2| -\frac{1}{2}} \\
\end{align}
$$