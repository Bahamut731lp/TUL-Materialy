# Příklad 2.2
**Spočtěte $\large\lim_{x\to\infty}\frac{x}{\ln^2(x^2)}$**


$$\Large
\begin{aligned}

& \lim_{x\to\infty}\frac{x}{\ln^2(x^2)} \\

=& \frac{\lim_{x\to\infty}x}{\lim_{x\to\infty}\ln^2(x^2)} \\

=& \frac{\infty}{\infty}

\\\\
&\text{It's L'Hospital Time:}
\\\\

&= \lim_{x\to\infty}\frac{1}{\frac{8}{x}\ln(x)} \\

&= \lim_{x\to\infty}\frac{x}{8\ln(x)} \\

&= \frac{1}{8}\lim_{x\to\infty}\frac{x}{\ln(x)} \\

&= \frac{1}{8}\lim_{x\to\infty}\frac{\infty}{\infty} \\

\\\\
&\text{It's L'Hospital Time:}
\\\\

&= \frac{1}{8}\lim_{x\to\infty}\frac{1}{\frac{1}{x}} \\

&= \frac{1}{8}\lim_{x\to\infty}x \\

&= \frac{1}{8}\infty \\

&= \boxed{\infty}
\end{aligned}
$$