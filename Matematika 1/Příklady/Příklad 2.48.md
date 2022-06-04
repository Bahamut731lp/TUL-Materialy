# Příklad 2.48
**Spočtěte $\Large\lim_{x\to1}\frac{\sin{(1-x)}}{(x^2-1)^2}$**


$$\Large
\begin{aligned}

&\lim_{x\to1}\frac{\sin{(1-x)}}{(x^2-1)^2} \\

=& \lim_{x\to1}\frac{0}{0} \\

\\\\
&\text{It's L'Hospital Time:}
\\\\

=& \lim_{x\to1}\frac{-\cos{(1-x)}}{4x^3-4x} \\

=& \lim_{x\to1}\frac{-\cos{(1-x)}}{4x^3-4x} \\

=& \lim_{x\to1}\frac{-1}{0} \\

\end{aligned}
$$

## Limity zleva a zprava
$$\Large
\begin{aligned}

&\lim_{x\to1}\frac{\sin{(1-x)}}{(x^2-1)^2} \\

\\\\

=& \lim_{x\to1^+}\frac{\text{\normalsize Vychází záporně}}{\text{\normalsize Vychází kladně}} \\

=& \lim_{x\to1^+}\text{\normalsize Vychází záporně} \\

\\\\

=& \lim_{x\to1^-}\frac{\text{\normalsize Vychází kladně}}{\text{\normalsize Vychází kladně}} \\

=& \lim_{x\to1^-}\text{\normalsize Vychází kladně} \\

\end{aligned}
$$

Limita zprava letí k $+\infty$, zatímco limita zprava k $-\infty$, limita tudíž neexistuje, protože se limita zleva nerovná limitě zprava.