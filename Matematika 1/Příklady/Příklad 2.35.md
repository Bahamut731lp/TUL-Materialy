# Příklad 2.35
**Spočtěte $\Large\lim_{x\to\infty}\frac{-2x^2+8}{e^{2x-1}}$**


$$\Large
\begin{aligned}

&\lim_{x\to\infty}\frac{-2x^2+8}{e^{2x-1}} \\

=& \lim_{x\to\infty}\frac{-2\cdot(x^2-4)}{e^{2x-1}} \\

=& \lim_{x\to\infty}\frac{-2\cdot(x-2)(x+2)}{e^{2x-1}} \\

=& \frac{\lim_{x\to\infty}-2\cdot(x-2)(x+2)}{\lim_{x\to\infty}e^{2x-1}} \\

=& \frac{-2\cdot\lim_{x\to\infty}(x-2)(x+2)}{e^{\lim_{x\to\infty}2x-1}} \\

=& \frac{-2\cdot\infty}{e^{\infty}} \\

=& -\infty \cdot \frac{1}{e^{\infty}}\\

=& -\infty \cdot 0\\

=& \;\boxed{0}


\end{aligned}
$$