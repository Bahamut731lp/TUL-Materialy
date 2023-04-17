
## Obor konvergence mocninné řady
Vytkněte, co se dá (hlavně konstanty a exponenty):
$$\large \sum_{n}^{\infty} (x-x_0)^{an+b}\cdot{c}^n = (x-x_0)^b \cdot \sum_{n}^{\infty} (x-x_0)^{an}+{c}^n$$
Vypočtetě střed konvergence:
$$\large S=-1 * x_0$$
Vypočtetě poloměr konvergence:
$$\Large r=(\lim_{n\to\infty}\sqrt[an]{c^n})^{-1} \text{ nebo } \left(\lim_{n\to\infty}\frac{a_{n+1}}{a_n}\right)^{-1}$$
Určete interval konvergence a došetřete krajní body pomocí klasických kritérií konvergence + dosazení:
$$\Large x\in\left(S-r,S+r\right)$$

## Limita dvou a více proměnných
Zkuste dosadit - jsou tři scénáře, co se může stát:
1. Limita výjde jako **reálné číslo** $\implies$ Limita existuje a tohle je výsledek
2. Limita výjde jako $\Large\frac{a}{0}, \normalsize a\in\mathbb{R} \implies$ V tomhle bodě je asymptota $\pm$ nekonečnu. O znaménku rozhoduje znaménko čísla $a$.
3. Limita výjde $\Large\frac{0}{0}, \normalsize\implies$ Musíme buďto zlomek nějak upravit, a nebo dokázat, že limita neexistuje.


Zkuste **dvojí limitu**
$$\Large \lim_{x\to\infty}(\lim_{y\to\infty}(a_n)) = \lim_{y\to\infty}(\lim_{x\to\infty}(a_n)) \implies \text{může existovat}$$

Zkuste se k bodu přiblížit po přímce, pokud ve výsledku zbyde $k$, je limita závislá na směrnici a limita neexistuje.
$$\Large y = k(x - x_0) + y_0$$
$$\Large \lim_{x\to\infty}f(x, k(x-x_0)+y_0)$$

Popř. se zkuste přiblížit po vhodné mocnině, či dokonce odmocnině.

## Derivace ve směru
- Výpočtěte derivace ve směru jako (skalární) součin vektoru gradientu a vektoru koeficientů směrového vektoru:
$$\Large\nabla{f}\cdot\vec{v}$$

- Vypočtěte [[Gradient]]:
$$\Large\nabla{f} = (f_x, f_{x_1}, f_{x_2}, ...)$$

- Vypočtěte hodnotu gradientu v zadaném bodě
$$\Large\nabla{f}(x, x_1, x_2, ...)$$

- Vypočtěte délku směrového vektoru
$$\Large|\vec{v}| = \sqrt{x^2 + (x_1)^2 + (x_2)^2 +\; ...}$$

- Normalizujte směrový vektor
$$\Large||\vec{v}|| = \left(\frac{v_1}{|\vec{v}|}, \frac{v_2}{|\vec{v}|},\;...\right)$$
- Vypočtěte [[Skalární součin]] normalizovaného směrového vektoru gradientu v zadaném bodě.
$$\Large ||\vec{v}|| \cdot \nabla{f}(x, x_1, x_2, ...)$$

## Tečná rovinna
$$\Large \tau: f(\vec{v_0})+\nabla{f}(\vec{v_0})\cdot(\vec{v}-\vec{v_0})$$

$$\Large \vec{v} = \begin{bmatrix}x \\ y\end{bmatrix}, \vec{v_0} = \begin{bmatrix}x_0 \\ y_0\end{bmatrix}, \vec{v}-\vec{v_0} = \begin{bmatrix}x - x_0 \\ y - y_0\end{bmatrix}$$

## Transformace diferenciálních výrazů
Jedná se akorát o derivaci složené funkce a substituci.

## Taylorův rozvoj
$$\Large\begin{aligned}
T_n = f(x_0, y_0) &+  \frac{1}{1!}d^1f(x_0,y_0)(h, k) 
\\&+ \frac{1}{2!}d^2f(x_0,y_0)(h, k) 
\\&+ \frac{1}{3!}d^3f(x_0,y_0)(h, k)
\\&...
\\&+ \frac{1}{n!}d^nf(x_0,y_0)(h, k)
\end{aligned}$$

$$\Large d^nf=\sum_{i=0}^{n}{n\choose i}f_{x^{n-i}y^{i}}(x_0,y_0)(x-x_0)^{n-i}(y-y_0)^i$$

kde:

|Proměnná|Význam|
|:--:|:--|
|$\large n$|Řádek [[Pascalův Trojúhelník\|Pascalova trojúhelníku]] |
|$\large i$|Sloupec [[Pascalův Trojúhelník\|Pascalova trojúhelníku]] |
|$\large f_{xy}$|Derivace podle x, y. Exponenty říkají, kolikrát se podle proměnné derivuje.|
|$\large (x_0, y_0)$|Bod, ve kterém děláme [[Taylorův Polynom]]|
|$\large d^nf$|Diferenciál $n$-tého řádu funkce $f$|