> [!example] Vypočtěte
> $$\Large \int_0^{\frac{1}{2}} 4x\cdot\arctan({2x})\;dx$$

> [!tip]- Aplikace [[Per Partes#Metoda DI|DI metody]]
> Sestavíme si DI tabulku:
>
>||D | I 
|:---:|:----------------:|:-------------:|
|+|$\arctan(2x)$ | $4x$ |
|-|$\frac{2}{4x^2+1}$|$2x^2$|
>Zapíšeme výsledek: $\arctan(2x)\cdot{2x^2}-\int_0^{\frac{1}{2}}\frac{2x^2}{4x^2 + 1}\cdot 2x^2\;dx$
$$
\large\begin{aligned}
&= \arctan(2x)\cdot{2x^2}-\int_0^{\frac{1}{2}}\frac{4x^2}{4x^2 + 1}\;dx
\end{aligned}
$$

> [!tip]+ Dělení polynomů
>
>$$\large\begin{aligned}
>4x^2 &: 4x^2 +1 = 1 - \frac{1}{4x^2+1}\\
>-(4x^2 + 1) \\
>-1 \\
>\end{aligned}$$

$$
\large\begin{aligned}
&= \arctan(2x)\cdot{2x^2}-\int_0^{\frac{1}{2}}1-\frac{1}{4x^2 + 1}\;dx \\
&= \arctan(2x)\cdot{2x^2}- x - \int_0^{\frac{1}{2}}\frac{1}{(2x)^2 + 1}\;dx \\
\end{aligned}
$$

> [!tip]- Substituce
>
>$$\large\begin{aligned}
u &= 2x \\
du &= 2dx \\
>\end{aligned}$$

$$\large\begin{aligned}
&= \arctan(2x)\cdot{2x^2}-x + \frac{1}{2}\int_0^{1}\frac{1}{u^2 + 1}\;du \\
&= \left[\arctan(2x)\cdot{2x^2}-x + \frac{1}{2}\arctan(2x)\right]^{\frac{1}{2}}_{0} \\
&= \left(\arctan(1)\cdot{2\left(\frac{1}{2}\right)^2} - \frac{1}{2} + \frac{1}{2}\arctan(1)\right) - \left(\arctan(0)\cdot{2\cdot0^2}-0 + \frac{1}{2}\arctan(0)\right) \\
&= \boxed{\arctan(1) - \frac{1}{2}}
\end{aligned}$$