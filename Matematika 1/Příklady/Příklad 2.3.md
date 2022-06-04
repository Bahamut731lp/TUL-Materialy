# Příklad 2.3
**Spočtěte  $\large\lim_{x\to5}\frac{(x+5)^2}{x^2-25}$**


$$\Large
\begin{aligned}

&\lim_{x\to5}\frac{(x+5)^2}{x^2-25} \\

=& \lim_{x\to5}\frac{(x+5)\cdot(x+5)}{(x+5)\cdot(x-5)} \\

=& \lim_{x\to5}\frac{\cancel{(x+5)}^1\cdot(x+5)}{\cancel{(x+5)}^1\cdot(x-5)} \\

=& \lim_{x\to5}\frac{(x+5)}{(x-5)} \\

=& \lim_{x\to5}\frac{(5+5)}{(5-5)} \\

=& \frac{10}{0} \; \text{\normalsize (Tohle smrdí asymptotou)} \\
\end{aligned}
$$

## Limity zleva a zprava
$$\Large
\begin{aligned}

&\lim_{x\to5}\frac{(x+5)}{(x-5)} \\
=& \lim_{x\to5^+}\frac{\text{vychází kladně}}{\text{vychází kladně}} &\text{\normalsize Pro čísla jako 5.1, 5.01, 5.001, ...} \\
=& \lim_{x\to5^+}\text{Kladné číslo} \\

\\\\\
=& \lim_{x\to5^-}\frac{\text{vychází kladně}}{\text{vychází záporně}} &\text{\normalsize Pro čísla jako 4.9, 4.99, 4.999, ...} \\
=& \lim_{x\to5^-}\text{Záporné číslo}
\end{aligned}
$$

Limita zprava a limita zleva nevychází jako stejné číslo, tudíž celková limita neexistuje.