
**Najděte inverzní funkci k funkci $f(x) = \frac{2-5\sin{(2x-1)}}{2}$ a určete definiční obory a obory hodnot tak, aby na těchto oborech byly tyto funkce navzájem inverzní.**

## Hledání inverzní funkce
$$\large\begin{aligned}

f(x): y &= \frac{2-5\sin{(2x-1)}}{2} \\
f^{-1}(x): x &= \frac{2-5\sin{(2y-1)}}{2} \\

\\\\

x &= \frac{2-5\sin{(2y-1)}}{2} && /\cdot 2\\
2x &= 2-5\sin{(2y-1)} && /-2\\
2x-2 &= -5\sin{(2y-1)} && /:(-5)\\
-\frac{2x-2}{5} &= \sin{(2y-1)} && /\arcsin{(x)} \\
\arcsin{\left(-\frac{2x-2}{5}\right)} &= 2y-1 && /+1\\
\arcsin{\left(-\frac{2x-2}{5}\right)} + 1 &= 2y && /:2\\
\frac{1}{2}\left(\arcsin{\left(\frac{2-2x}{5}\right)} + 1\right) &= y\\
\boxed{\frac{1}{2}\left(\arcsin{\left(\frac{2-2x}{5}\right)} + 1\right)} &= y

\end{aligned}$$

## Určení oborů

Interval prostosti funkce $\text{arcsin}(x)$ je $\left(0,1\right)$.

$$\large D(f) = H(f^{-1}) = \left<\frac{2-\pi}{4}, \frac{2+\pi}{4}\right>$$
$$\large D(f^{-1}) = H(f) = \left<-\frac{3}{2}, \frac{7}{2}\right>$$

---

$$\large\begin{aligned}
-\frac{\pi}{2} &\le 2x-1 &\le \frac{\pi}{2} \\
-\frac{\pi}{2}+1 &\le 2x &\le \frac{\pi}{2}+1 \\
-\frac{\pi}{4}+\frac{1}{2} &\le x &\le \frac{\pi}{4}+\frac{1}{2} \\
\frac{2-\pi}{4} &\le x &\le \frac{2+\pi}{4}
\\\\

x &\in \boxed{\left<\frac{2-\pi}{4}, \frac{2+\pi}{4}\right>}
\end{aligned}$$

---
$$\large\begin{aligned}
-1 &\le \frac{2-2x}{5} &\le 1 \\
-5 &\le 2-2x &\le 5 \\
-7 &\le -2x &\le 3 \\
-\frac{7}{2} &\le -x &\le \frac{3}{2}\\
\frac{7}{2} &\ge x &\ge -\frac{3}{2}\\

\\\\

x &\in \boxed{\left<-\frac{3}{2}, \frac{7}{2}\right>}
\end{aligned}$$
