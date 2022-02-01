# Triky pro derivaci
V tomhle dokumentu najdete pár triků pro rychlejší derivace.

## Derivace převrácené hodnoty
Tenhle trik je zkrácená verze [[Pravidla pro práci s derivacemi#Derivování operací|derivace podílu]].
$\huge\frac{d}{dx}(\frac{a}{f(x)}) = \frac{-a\cdot f'(x)}{f(x)^2}$

## Derivace stejných funkcí v podílu
$\huge\frac{d}{dx}(\frac{a \cdot f(x) + b}{c \cdot f(x) + d}) = \frac{f'(x) \cdot (ad-bc)}{(c \cdot f(x)+d)^2}$

## Derivace mocniny
$\huge\frac{d}{dx}(\sqrt{f(x)}) = \frac{f'(x)}{2\sqrt{f(x)}}$

## Derivace pomocí logaritmů
Pokud máme podíl dvou polynomů (a klidně i jiných pěkných funkcí k logaritmování), tak stojí za zvážení použití vlastností logaritmů k našemu prospěchu

$$\Large\begin{aligned}
y &= \frac{x^2(x+1)}{(x-3)^4} \\
\ln(y) &= \ln({ \frac{x^2(x+1)}{(x-3)^4} }) \\
\ln(y) &= 2\ln(x)+\ln(x+1)-4\ln(x-3) \\
\frac{y'}{y} &= \frac{2}{x} + \frac{1}{x+1} - \frac{4}{x-3} \\
\frac{y'}{y} &= \left( \frac{2}{x} + \frac{1}{x+1} - \frac{4}{x-3} \right) \cdot y \\
y' &= \left( \frac{2}{x} + \frac{1}{x+1} - \frac{4}{x-3} \right) \cdot \frac{x^2(x+1)}{(x-3)^4} \\
\end{aligned}$$