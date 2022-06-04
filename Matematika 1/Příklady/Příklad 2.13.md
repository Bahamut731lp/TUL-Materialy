# Příklad 2.13
**Spočtěte limitu posloupnosti $\Large\lim_{n\to\infty}\frac{3n+2n^2}{2-n}$**


$$\Large
\begin{aligned}

&\lim_{n\to\infty}\frac{3n+2n^2}{2-n} \\

=& \lim_{n\to\infty}\frac{n^2\cdot(\frac{3}{n}+2)}{n\cdot(\frac{2}{n^2}-1)} \\

=& \lim_{n\to\infty}\frac{\cancel{n^2}^{n}\cdot(\frac{3}{n}+2)}{\cancel{n}^{1}\cdot(\frac{2}{n^2}-1)} \\

=& \lim_{n\to\infty}\frac{\cancel{n^2}^{n}\cdot\left(\frac{3}{n}+2\right)}{\cancel{n}^{1}\cdot(\frac{2}{n^2}-1)} \\

=& \lim_{n\to\infty}\frac{n\cdot\left(\cancel{\frac{3}{n}}^{\lim\to0}+2\right)}{\cancel{\frac{2}{n^2}}^{\lim\to0}-1} \\

=& \lim_{n\to\infty}\frac{n\cdot2}{-1} \\

=& \boxed{-\infty}

\end{aligned}
$$