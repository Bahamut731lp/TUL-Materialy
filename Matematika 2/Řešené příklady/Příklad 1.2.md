**Určete obor konvergence řady $\Large\sum_{n=1}^{\infty}(x-9)^n3^{(2-2n)}n$**

Střed konvergence: $\large x-9=0 \implies x=9$

Nalezení poloměru konvergence - použití převráceného odmocninového kritéria:
$$\large\begin{aligned}

r &= \left(\lim_{n\to\infty} \sqrt[n]{3^{(2-2n)}n}\right)^{-1} 

\\&= \left(\lim_{n\to\infty}\sqrt[n]{3^{2}}\cdot\sqrt[n]{3^{-2n}}\cdot \sqrt[n]{n}\right)^{-1}

\\&=\left(\lim_{n\to\infty}1\cdot\frac{1}{\sqrt[n]{3^{2n}}}\cdot 1\right)^{-1}

\\&=\left(\lim_{n\to\infty}\frac{1}{9}\right)^{-1}

\\&=\left(\frac{1}{9}\right)^{-1}

\\&= 9
\end{aligned}$$
Z toho vyplývá $\large x\in\left(0,9\right)$

---
Vyšetření v krajních bodech:

$\large x=0: \sum_{n=1}^{\infty}\sqrt[n]{-9^n\cdot3^{(2-2n)}n}$


Použití odmocninového kritéria:
$$\large \begin{aligned}

\lim_{n\to\infty}\sqrt[n]{(-9)^{n}3^{2-2n}} 

&= \lim_{n\to\infty}\sqrt[n]{(-9)^{n}}\cdot\sqrt[n]{3^{2-2n}}\cdot\sqrt[n]{n} 

\\&=-\lim_{n\to\infty}9\cdot{1}\cdot\sqrt[n]{3^{2}}\cdot\sqrt[n]{3^{-2n}}\cdot 1 

\\&=-\lim_{n\to\infty}9\cdot{1}\cdot1\cdot\frac{1}{9}\cdot 1 

\\&=-\lim_{n\to\infty}9

\\&=-9

\\-9 &\lt1 \implies \text{Patří do intervalu konvergence}
\end{aligned}
$$
Výsledný interval konvergence: $\large x \in \left<0,4\right)$