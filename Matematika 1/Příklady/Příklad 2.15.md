# Příklad 2.15
**Spočtěte $\Large\lim_{x\to3}\frac{x^2-4x+3}{(9-x^2)^2}$**

$$\Large
\begin{aligned}

&\lim_{x\to3}\frac{x^2-4x+3}{(9-x^2)^2} \\

=& \lim_{x\to3}\frac{12-12}{0^2} \\

=& \frac{0}{0} \\

\\\\
&\text{It's L'Hospital Time:}
\\\\

=& \lim_{x\to3}\frac{2x-4}{2(9-x^2)(-2x)} \\

=& \lim_{x\to3}\frac{2x-4}{2(9-x^2)(-2x)} \\

=& \lim_{x\to3}\frac{2x-4}{-4x(9-x^2)} \\

=& \lim_{x\to3}\frac{6-4}{-12\cdot(0)} \\

=& \frac{2}{0} \\

\end{aligned}
$$

## Limity zleva a zprava
$$\Large
\begin{aligned}

&\lim_{x\to3}\frac{x^2-4x+3}{(9-x^2)^2} \\

=& \lim_{x\to3}\frac{2x-4}{-4x(9-x^2)} \\

\\\\

=& \lim_{x\to3^+}\frac{2x-4}{-4x(9-x^2)} \\

=& \lim_{x\to3^+}\frac{\text{\normalsize Vychází kladně}}{\text{\normalsize Vychází záporně} \cdot (\text{\normalsize Vychází záporně})} \\

=& \lim_{x\to3^+}\frac{\text{\normalsize Vychází kladně}}{\text{\normalsize Vychází kladně}} \\

=& \lim_{x\to3^+}{\text{\normalsize Vychází kladně}} \\

\\\\

=& \lim_{x\to3^-}\frac{2x-4}{-4x(9-x^2)} \\

=& \lim_{x\to3^+}\frac{\text{\normalsize Vychází kladně}}{\text{\normalsize Vychází záporně} \cdot (\text{\normalsize Vychází kladně})} \\

=& \lim_{x\to3^+}\frac{\text{\normalsize Vychází kladně}}{\text{\normalsize Vychází záporně}} \\

=& \lim_{x\to3^+}{\text{\normalsize Vychází záporně}} \\

\end{aligned}
$$

Limita zprava letí k $-\infty$, zatímco limita zprava k $+\infty$, limita tudíž neexistuje, protože se limita zleva nerovná limitě zprava.