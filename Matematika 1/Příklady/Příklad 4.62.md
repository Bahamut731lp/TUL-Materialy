> [!example] Vypočtěte
> $$\Large \int_{0}^{1} \frac{1}{(1+x^2)\cdot\sqrt{\arctan(x)}}\;dx$$

> [!tip]+ Substituce
>
>$$\large\begin{aligned}
u &= \arctan{x} \\
du &= \frac{1}{x^2+1}dx \\
>\end{aligned}$$

$$\large
\begin{align}
	&= \int_{0}^{\frac{\pi}{4}} \frac{1}{\sqrt{u}}\;du \\
	&= \int_{0}^{\frac{\pi}{4}} u^{-\frac{1}{2}}\;du \\
	&= \left[\frac{u^{\frac{1}{2}}}{\frac{1}{2}}\right]_{0}^{\frac{\pi}{4}} \\
	&= \left[2u^{\frac{1}{2}}\right]_{0}^{\frac{\pi}{4}} \\
	&= 2\sqrt{\frac{\pi}{4}}\\
	&= \cancel{2}^1{\frac{\sqrt{\pi}}{\cancel{2}^1}}\\
	&= \boxed{\sqrt{\pi}}\\
\end{align}
$$