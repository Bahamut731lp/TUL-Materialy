# Příklad 2.11
**Spočtěte $\Large\lim_{x\to0}\frac{(\cos^2{x}-1)^2}{x^4}$**


$$\Large
\begin{aligned}

&\lim_{x\to0}\frac{(\cos^2{x}-1)^2}{x^4} &\normalsize(\sin^2{x}+\cos^2{x} =1)\\

=& \lim_{x\to0}\frac{(-1\cdot(1-\cos^2{x}))^2}{x^4} \\

=& \lim_{x\to0}\frac{(-1\cdot\sin^2{x})^2}{x^4} \\

=& \lim_{x\to0}\frac{(-\sin^2{x})^2}{x^4} & \text{\normalsize Cokoliv na 2 bude kladné} \\

=& \lim_{x\to0}\frac{\sin^4{x}}{x^4} \\

=& \lim_{x\to0}\left(\frac{\sin{x}}{x}\right)^4 \\

=& \left(\lim_{x\to0}\frac{\sin{x}}{x}\right)^4 & \text{\normalsize Tohle je známá limita, nebo se dá odvodit}\\

=& \left(\frac{0}{0}\right)^4 \\

\\\\
&\text{It's L'Hospital Time:}
\\\\

=& \left(\lim_{x\to0}\frac{\cos{x}}{1}\right)^4 \\

=& \left(\lim_{x\to0}\cos{x}\right)^4 \\

=& \left(1\right)^4 \\

=& \boxed{1}

\end{aligned}
$$