# Příklad 2.1
**Spočtěte limitu posloupnosti $\large\lim_{n\to\infty}\frac{1+2n+5n^2}{2n-n^2}$**


$$\Large
\begin{aligned}

& \lim_{n\to\infty}\frac{1+2n+5n^2}{2n-n^2} \\

=& \lim_{n\to\infty}\frac{n^2\cdot(\frac{1}{n^2}+\frac{2}{n}+5)}{n^2\cdot(\frac{2}{n}-1)} \\

=& \lim_{n\to\infty}\frac{\cancel{n^2}^1\cdot(\frac{1}{n^2}+\frac{2}{n}+5)}{\cancel{n^2}^1\cdot(\frac{2}{n}-1)} \\

=& \lim_{n\to\infty}\frac{\frac{1}{n^2}+\frac{2}{n}+5}{\frac{2}{n}-1} \\

=& \frac{\lim_{n\to\infty}(\frac{1}{n^2}+\frac{2}{n}+5)}{\lim_{n\to\infty}(\frac{2}{n}-1)} \\

=& \frac{\lim_{n\to\infty}(\frac{1}{n^2})+\lim_{n\to\infty}(\frac{2}{n})+\lim_{n\to\infty}(5)}{\lim_{n\to\infty}(\frac{2}{n})-\lim_{n\to\infty}(1)} \\

=& \frac{0+0+5}{0-1} \\

=& \frac{+5}{-1} \\

=& \boxed{-5}

\end{aligned}
$$