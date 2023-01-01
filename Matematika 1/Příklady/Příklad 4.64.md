> [!example] Vypočtěte
> $$\Large \int_{0}^{\pi} 2x^2\cdot\cos(2x)\;dx$$

$$\large
\begin{align}
	&= \int_{0}^{\pi} x^2\cdot\cos(2x)\;2dx \\
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
	&= \int_{0}^{2\pi} \left(\frac{u}{2}\right)^2\cdot\cos(u)\;du \\
	&= \int_{0}^{2\pi} \frac{1}{4}u^2\cdot\cos(u)\;du \\
	&= \frac{1}{4}\int_{0}^{2\pi} u^2\cdot\cos(u)\;du \\
\end{align}
$$

> [!tip]+ Aplikace [[Per Partes#Metoda DI|DI metody]]
> Sestavíme si DI tabulku:
>
>||D | I 
|:---:|:----------------:|:-------------:|
|+|$u^2$ | $\cos(u)$ |
|-|$2u$|$\sin(u)$|
|+|$2$|$-\cos(u)$|
|-|$0$|$-\sin(u)$|
>Zapíšeme výsledek: $u^2\sin(u)+2u\cos(u)-2\sin(u)$

$$\large
\begin{align}
	&= \frac{1}{4}\left[u^2\sin(u)+2u\cos(u)-2\sin(u)\right]_{0}^{2\pi} \\
	&= \frac{1}{4}\left[4\pi\right] \\
	&= \boxed{\pi}
\end{align}
$$