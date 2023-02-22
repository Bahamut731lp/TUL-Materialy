> [!example] Spočtěte obsah obrazce
> ohraničeného funkcemi $x\cdot\sin{x}$ a $x\cdot(x-\pi)$

>[!info]
>$$\begin{aligned}
>f(x) &= x\cdot\sin{x} \\
>g(x) &= x\cdot(x-\pi)
>\end{aligned}$$

>[!info] Vypočítání [[Integrační meze]]
>- Obě funkce se budou rovnat v nule, protože budeme v obou násobit nulou.
>- Když pak vynecháme vnější $x$ a podíváme, kdy se funkce znovu rovnají nule, tak pro 
>	- $\sin(x) = 0$ pro $x=k\pi$
>	- $x-\pi = 0$ pro $x = \pi$
>- Můžeme tedy zvolit interval $\left<0, \pi\right>$
$$
\begin{aligned}
	&= \int_{0}^{\pi} f(x) - g(x)\;dx \\
	&= \int_{0}^{\pi} x\cdot\sin{x}\;dx - \int_{0}^{\pi}x\cdot(x-\pi)\;dx \\
	&= \int_{0}^{\pi} x\cdot\sin{x}\;dx - \int_{0}^{\pi}x^2\;dx+\int_{0}^{\pi}x\pi\;dx \\
\end{aligned}
$$

> [!tip]+ Aplikace [[Per Partes#Metoda DI|DI metody]]
> Sestavíme si DI tabulku:
>
>||D | I 
|:---:|:----------------:|:-------------:|
|+|$x$ | $\sin{x}$ |
|-|$1$|$-\cos{x}$|
|+|0|$-\sin{x}$|
>Zapíšeme výsledek: $x\cdot(-\cos{x})-1\cdot(-\sin{x}) = -x\cdot\cos{x}+\sin{x}$

$$
\begin{aligned}
	&= \int_{0}^{\pi} x\cdot\sin{x}\;dx - \int_{0}^{\pi}x^2\;dx+\int_{0}^{\pi}x\pi\;dx \\
	&= \left[-x\cdot\cos{x}+\sin{x}\right]_{0}^{\pi}-
	\left[\frac{x^3}{3}\right]_{0}^{\pi}
	+\pi\cdot \left[\frac{x^2}{2}\right]_{0}^{\pi} \\
	&= \left[-\pi\cdot\cos{\pi}+\sin{\pi} - 0\cdot\cos(0)+\sin(0)\right] - \left[\frac{\pi^3}{3} - \frac{0}{3}\right] + \pi\cdot\left[\frac{\pi^2}{2} - \frac{0}{2}\right] \\
	&= \left[-\pi\cdot{-1}+0 - 0\cdot1+0\right] - \frac{\pi^3}{3} + \pi\cdot\frac{\pi^2}{2} \\
	&= \pi- \frac{\pi^3}{3} + \frac{\pi^3}{2} \\
	&= \pi - \frac{2\pi^3}{6} + \frac{3\pi^3}{6} \\
	&= \boxed{\pi + \frac{\pi^3}{6}}
\end{aligned}
$$

