# Příklad 2.53
**Spočtěte $\Large\lim_{x\to0}\frac{\sqrt[3]{1-x}-1}{x}$**


$$\Large
\begin{aligned}

&\lim_{x\to0}\frac{\sqrt[3]{1-x}-1}{x} \\

=& \lim_{x\to0}\frac{(1-x)^{\frac{1}{3}}-1}{x} \\

=& \lim_{x\to0}\frac{1-1}{0} \\

=& \frac{0}{0} \\

\\\\
&\text{It's L'Hospital Time:}
\\\\

=& \lim_{x\to0}\frac{(1-x)^{\frac{1}{3}}-1}{x} \\

=& \lim_{x\to0}\frac{\frac{1}{3}(1-x)^{-\frac{2}{3}}\cdot(-1)}{1} \\

=& \lim_{x\to0}-\frac{1}{3}(1-x)^{-\frac{2}{3}} \\

=& \lim_{x\to0}-\frac{1}{3}\left(\sqrt[3]{(1-x)^2}\right)^{-1} \\

=& \lim_{x\to0}-\frac{1}{3}\left(\sqrt[3]{(1-0)^2}\right)^{-1} \\

=& \lim_{x\to0}-\frac{1}{3}\left(\sqrt[3]{1}\right)^{-1} \\

=& \lim_{x\to0}-\frac{1}{3}\cdot{1} \\

=& \boxed{-\frac{1}{3}}

\end{aligned}
$$