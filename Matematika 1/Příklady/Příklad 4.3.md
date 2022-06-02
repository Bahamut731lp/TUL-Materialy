# Příklad 4.3
$$\large\begin{aligned}
&\int_{-\frac{\pi}{2}}^{0}\frac{\sin{x}\cos{x}}{25+10\sin{x}+\sin^2{x}} \; dx = \int_{-\frac{\pi}{2}}^{0}\frac{\sin{x}\cos{x}}{(5+\sin^2{x})} \; dx \\
\end{aligned}$$

## Výpočet neurčitého integrálu:
---
Substituce:

$$\large
\begin{aligned}
u &= \sin{x} \\
du &= \cos{x} \; dx \\
\end{aligned}
$$

---

$$\large\begin{aligned}
&=\int \frac{\sin{x}}{(5+\sin{x})^2} (\cos{x}\;dx) \\
&= \int \frac{u}{(5+u)^2} \;du \\
\end{aligned}$$

---
Substituce:

$$\large
\begin{aligned}
v &= 5+u \\
v &= 5 + \sin{x} \\
dv &= du \\

\implies u &=v-5
\end{aligned}
$$

---

$$\large\begin{aligned}
&= \int \frac{u}{(5+u)^2} \;du \\

&= \int \frac{v - 5}{v^2} \; dv \\

&= \int \frac{v}{v^{2}} - \frac{5}{v^2} dv \\

&= \int \frac{1}{v} - 5\int \frac{1}{v^2} dv \\

&= \ln{|v|} - 5\int v^{-2} dv \\

&= \ln{|v|} - 5\cdot \left(\frac{v^{-1}}{-1}\right) \\

&= \ln{|v|} + \frac{5}{v} \\

&= \boxed{\ln{|5 + \sin{x}|} + \frac{5}{5 + \sin{x}}}
\end{aligned}$$

## Výpočet určitého integrálu
$$\large\begin{aligned}

&\int_{-\frac{\pi}{2}}^{0}\frac{\sin{x}\cos{x}}{25+10\sin{x}+\sin^2{x}} \; dx = \left[\ln{|5 + \sin{x}|} + \frac{5}{5 + \sin{x}}\right]_{-\frac{\pi}{2}}^{0} \\

&= \ln{|5 + \sin{0}|} + \frac{5}{5 + \sin{0}} - \ln{|5 + \sin{-\frac{\pi}{2}}|} - \frac{5}{5 + \sin{-\frac{\pi}{2}}} \\

&= \ln{5} + \frac{\cancel{5}^1}{\cancel{5}^1} - \ln{|5 + (-1)|} - \frac{5}{5 + (-1)} \\

&= \ln{5} + 1 - \ln{4} - \frac{5}{4} \\

&= \boxed{\ln{\frac{5}{4}} - \frac{1}{4}}

\end{aligned}$$