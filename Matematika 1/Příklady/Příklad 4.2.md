# Příklad 4.2
$$\large\begin{aligned}
&\int_{0}^{1}\frac{x^4}{(e^{x^5})^5} \; dx = \int_{0}^{1}\frac{x^4}{e^{5x^5}} \; dx = \\
\end{aligned}$$

## Výpočet neurčitého integrálu:
---
Substituce:

$$\large
\begin{aligned}
u &= x^5 \\
du &= 5x^4 \; dx \\
\end{aligned}
$$

Přidání koeficinetu $5$ k $x^4$, aby se lépe substituovalo :
$$\large\begin{aligned}
&\int\frac{x^4}{e^{5x^5}} \; dx = \frac{1}{\cancel{5}}\int\frac{\cancel{5}x^4}{e^{5x^5}} \; dx\\
\end{aligned}$$

---
$$\large\begin{aligned}
&= \frac{1}{5}\int\frac{1}{e^{5x^5}} (5x^4 \; dx) \\

&= \frac{1}{5}\int\frac{1}{e^{5u}} \; du \\

&= \frac{1}{5}\int e^{-5u} \; du \\

&= \frac{1}{5}\cdot\left(-\frac{1}{5}e^{-5u}\right) \\

&= -\frac{1}{25}e^{-5u} \\

&= \boxed{-\frac{1}{25}e^{-5x^5}} \\
\end{aligned}$$

## Výpočet určitého integrálu
$$\large\begin{aligned}
&\int_{0}^{1}\frac{x^4}{(e^{x^5})^5} \; dx = \left[-\frac{1}{25}e^{-5x^5}\right]_{0}^{1}\\

&= -\frac{1}{25}e^{-5\cdot1^5} - \left(-\frac{1}{25}e^{-5\cdot 0^5}\right) \\

&= -\frac{1}{25}e^{-5} + \frac{1}{25}e^{0} \\

&= -\frac{e^{-5}}{25} + \frac{1}{25} \\

&= \frac{-e^{-5} + 1}{25} \\

&= \boxed{\frac{1 - e^{-5}}{25}}
\end{aligned}$$