**Určete obor konvergence řady $\Large\sum_{n=1}^{\infty}(x-2)^n2^{(1-n)}n^{-1}$**

Střed konvergence: $\large x-2=0 \implies x=2$

Nalezení poloměru konvergence - použití převráceného odmocninového kritéria:
$$\large\begin{aligned}

r &= \left(\lim_{n\to\infty} \sqrt[n]{2^{1-n}n^{-1}}\right)^{-1} 

\\&= \left(\lim_{n\to\infty}\sqrt[n]{2}\cdot\sqrt[n]{\frac{1}{2^n}}\cdot\sqrt[n]{\frac{1}{n}}\right)^{-1}

\\&=\left(\lim_{n\to\infty}1\cdot{\frac{\sqrt[n]{1}}{\sqrt[n]{2^n}}}\cdot{\frac{\sqrt[n]{1}}{\sqrt[n]{n}}}\right)^{-1}

\\&=\left(\lim_{n\to\infty}1\cdot{\frac{1}{2}}\cdot{\frac{1}{1}}\right)^{-1}

\\&=\left(\frac{1}{2}\right)^{-1}

\\&= 2
\end{aligned}$$
Z toho vyplývá $\large x\in\left(0,4\right)$

---
Vyšetření v krajních bodech:

$\large x=0: \sum_{n=1}^{\infty}(-2)^{n}2^{1-n}n^{-1}$

Použití odmocninového kritéria:
$$\large \begin{aligned}

\lim_{n\to\infty}\sqrt[n]{(-2)^{n}2^{1-n}n^{-1}} 

&= \lim_{n\to\infty}\sqrt[n]{(-2)^{n}}\cdot\sqrt[n]{2^{1-n}}\cdot\sqrt[n]{n^{-1}} 

\\&=\lim_{n\to\infty}-2\cdot\sqrt[n]{2^{1}}\sqrt[n]{2^{-n}}\cdot 1 

\\&=\lim_{n\to\infty}-2\cdot 1 \cdot \frac{1}{2}\cdot 1

\\&=\lim_{n\to\infty}-1

\\&=-1

\\-1 &\lt1 \implies \text{Patří do intervalu konvergence}
\end{aligned}
$$


$\large x=4: \sum_{n=1}^{\infty}2^{n}2^{1-n}n^{-1}$
$$\large \begin{aligned}

\lim_{n\to\infty}\sqrt[n]{(2)^{n}2^{1-n}n^{-1}} 

&= \lim_{n\to\infty}\sqrt[n]{(2)^{n}}\cdot\sqrt[n]{2^{1-n}}\cdot\sqrt[n]{n^{-1}} 

\\&=\lim_{n\to\infty}2\cdot\sqrt[n]{2^{1}}\sqrt[n]{2^{-n}}\cdot 1 

\\&=\lim_{n\to\infty}2\cdot 1 \cdot \frac{1}{2}\cdot 1

\\&=\lim_{n\to\infty}1

\\&=1

\\1 &\not\lt1 \implies \text{Nepatří do intervalu konvergence}
\end{aligned}
$$

Výsledný interval konvergence: $\large x \in \left<0,4\right)$

---
Btw:
$$\Large\lim_{n\to\infty}\sqrt[n]{n} = n^{\frac{1}{n}}=\lim_{n\to\infty}n^{\lim_{n\to\infty}\frac{1}{n}}=\lim_{n\to\infty}n^0=1$$
K tomuto výsledku lze dospět i použitím exponenciál na přirozený logaritmus, ale to je zdlouhavější :)