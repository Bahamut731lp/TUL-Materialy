# Příklad 4.1

$$\large\begin{aligned}
&\int_{0}^{\frac{1}{2}}4x \arctan{2x} \; dx = 4\int x \arctan{2x} \; dx
\end{aligned}$$

---
Per Partes:

|Znaménko|D|I|
|:--:|:--:|:--:|
|+|$\arctan(2x)$|$x$|
|-|$\large\frac{2}{1+4x^2}$|$\frac{1}{2}x^2$|

---

$$\large
\begin{aligned}
&=4\cdot\left(\frac{1}{2}\arctan(2x)x^2 - \int \frac{2}{1+4x^2} \frac{1}{2}x^2 \; dx\right)
\end{aligned}$$

---
Dělení polynomů:
$$
\large \frac{x^2}{4x^2+1} = \frac{1}{4}\text{, zbytek} \left(-\frac{1}{4}\cdot\frac{1}{4x^2+1}\right)
$$
---

$$\large
\begin{aligned}
&= 4\cdot\left(\frac{1}{2}\arctan(2x)x^2 - \left(\int \frac{1}{4} - \frac{1}{4}\cdot\frac{1}{4x^2+1} \; dx \right)\right) \\

&= 4\cdot\left(\frac{1}{2}\arctan(2x)x^2 -\left(\int \frac{1}{4} \; dx - \int \frac{1}{4}\cdot \frac{1}{4x^2+1} \; dx \right)\right) \\

&= 4\cdot\left(\frac{1}{2}\arctan(2x)x^2 -\left(\frac{1}{4}\int 1 \; dx - \frac{1}{4}\int \frac{1}{4x^2+1} \; dx \right)\right) \\

&= 4\cdot\left(\frac{1}{2}\arctan(2x)x^2 -\frac{1}{4}x + \frac{1}{4}\int \frac{1}{4x^2+1} \; dx \right)

\end{aligned}$$

---
**Výpočet vnořeného integrálu**
$$\large\int \frac{1}{4x^2+1} \; dx$$

Substituce:
$$\large
\begin{aligned}
u &= 2x \\
du &= 2dx \\
dx &= \frac{du}{2}
\end{aligned}
$$

$$\large\begin{aligned}
\large\int \frac{1}{4x^2+1} \; dx &= \\
&=\int \frac{1}{u^2+1} \; \frac{du}{2} \\
&= \frac{1}{2} \int \frac{1}{u^2+1} \; du \\
&= \frac{1}{2} \arctan(u) \\
&= \frac{1}{2} \arctan(2x)
\end{aligned}
$$
---

$$\large
\begin{aligned}

&= 4\cdot\left(\frac{1}{2}\arctan(2x)x^2 -\frac{1}{4}x + \frac{1}{4}\cdot\frac{1}{2}\arctan(2x) \right) \\

&= 4\cdot\left(\frac{1}{2}\arctan(2x)x^2 -\frac{1}{4}x + \frac{1}{8}\arctan(2x) \right) \\

&= \boxed{2x^2\arctan(2x) -x + \frac{1}{2}\arctan(2x)}
\end{aligned}$$

---
**Výpočet určitého integrálu**:
$$\large\begin{aligned}
&\int_{0}^{\frac{1}{2}}4x \arctan{2x} \; dx = \left[2x^2\arctan(2x) -x + \frac{1}{2}\arctan(2x)\right]_{0}^{\frac{1}{2}} \\

&= \left(2\left(\frac{1}{2}\right)^2\arctan\left(2\frac{1}{2}\right) -\frac{1}{2} + \frac{1}{2}\arctan\left(2\frac{1}{2}\right)\right) - 0 \\

&= \left(\frac{2}{4}\arctan\left(\frac{2}{2}\right) -\frac{1}{2} + \frac{1}{2}\arctan\left(\frac{2}{2}\right)\right) \\

&= \underline{\frac{1}{2}\arctan(1)} -\frac{1}{2} + \underline{\frac{1}{2}\arctan(1)} \\

&= \boxed{\arctan(1) - \frac{1}{2}}

\end{aligned}$$