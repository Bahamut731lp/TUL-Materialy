>[!example] Najděte inverzní funkci k funkci $f(x)$ a určete definiční obory a obory hodnot tak, aby na těchto oborech byly tyto funkce navzájem inverzní.
>$$\large f(x) = \frac{2-\text{arccotg}(x-1)}{5}$$

## Hledání inverzní funkce
$$\large\begin{aligned}

f(x): y &= \frac{2-\text{arccotg}(x-1)}{2} \\
f^{-1}(x): x &= \frac{2-\text{arccotg}(y-1)}{2} \\

\\\\

x &= \frac{2-\text{arccotg}(y-1)}{2} && /\cdot 2\\
2x &= 2-\text{arccotg}(y-1) && /-2\\
2x-2 &= -\text{arccotg}(y-1) && /\cdot(-1)\\
-2x+2 &= \text{arccotg}(y-1) && /\cot(x)\\
\text{cotg}(-2x+2) &= y-1 &&/+1 \\
y &= \boxed{\text{cotg}(-2x+2) + 1}

\end{aligned}$$

## Určení oborů

Interval prostosti funkce $\text{cotg}(x)$ je $\left(0\pi,1\pi\right)$.

$$\large D(f) = H(f^{-1}) = \mathbb{R}$$
$$\large D(f^{-1}) = H(f) = \left(\frac{2-\pi}{2}, 1\right)$$

---

$$\large\begin{aligned}
0\pi &< -2x+2 &< \pi \\
- 2 &< -2x &< \pi - 2 \\
\frac{-2}{2} &< -x &< \frac{\pi - 2}{2} \\
\frac{-2}{2} &> x &> -\frac{\pi - 2}{2} \\
1 &> x &> \frac{2-\pi}{2} \\

\\\\

x &\in \boxed{\left(\frac{2-\pi}{2}, 1\right)}
\end{aligned}$$