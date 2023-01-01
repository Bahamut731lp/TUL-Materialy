**Spočtěte limitu $\large\lim_{x\to0^+}\sqrt{x}\ln(x)$**


$$\Large
\begin{aligned}

& \lim_{x\to0^+}\sqrt{x}\ln(x) \\

=& \lim_{x\to0^+}\frac{\ln(x)}{\frac{1}{\sqrt{x}}} \\
=& \lim_{x\to0^+}-\frac{\infty}{\infty} \\

\\\\
&\text{It's L'Hospital Time:}
\\\\

=& \lim_{x\to0^+} \frac{(\ln(x))^{'}}{\left(\frac{1}{\sqrt{x}}\right)^{'}} \\
=& \lim_{x\to0^+} \frac{\frac{1}{x}}{-\frac{1}{2}x^{-\frac{3}{2}}} \\
=& \lim_{x\to0^+} \frac{1}{x}\cdot\frac{-2}{x^{-\frac{3}{2}}} \\
=& \lim_{x\to0^+} \frac{1}{x}\cdot(-2x^{\frac{3}{2}}) \\
=& \lim_{x\to0^+} \frac{1}{x}\cdot(-2\cdot{x^1}\cdot{}x^{\frac{1}{2}}) \\
=& \lim_{x\to0^+} \frac{1}{\cancel{x}^1}\cdot(-2\cdot\cancel{{x^1}}^1\cdot{}x^{\frac{1}{2}}) \\
=& \lim_{x\to0^+} (-2x^{\frac{1}{2}}) \\
=& \lim_{x\to0^+} -2 \cdot \lim_{x\to0^+} x^{\frac{1}{2}} \\
=& -2 \cdot 0 \\
=& \boxed{0}

\end{aligned} \\
$$