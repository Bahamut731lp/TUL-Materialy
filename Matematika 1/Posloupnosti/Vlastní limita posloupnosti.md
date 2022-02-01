# Limita posloupnosti
Posloupnost $\{a_n\}_{n=1}^{\infty}$ má (vlastní) limitu v bodě $a$, pokud pro libovolně velké [[Okolí bodu|okolí]] platí, že rozdíl prvku a limity je menší než okolí.

>**Definice  vlastní limity posloupnosti:**
>Posloupnost má vlastní limitu v oboru reýlných čísel, jestliže pro každé [[Okolí bodu|okolí]] epsilon existuje pořadové číslo (index) $n_0$, od kterého každy prvek s vyšším pořadovým číslem spadá do prostoru ohraničeného okolím epsilon.
>
>![[Pasted image 20211210135426.png]]

>**Jednoznačnost limity posloupnosti:**
>Každá posloupnost může mít nejvýše jednu limitu.

## Konvergence a divergence
**Konvergence**
Pokud  posloupnost má vlastní limitu, tak se body sbíhají k sobě. V tomto případě říkáme, že posloupnost **konverguje** (k bodu limity). 

$$\Large\lim_{n\to\infty} a_n = a$$

**Divergence**
Pokud  posloupnost nemá vlastní limitu, tak říkáme, že posloupnost **diverguje**. 

## Kdy limita neexistuje
Limita posloupnosti neexistuje v případě, kdy najdeme dvě [[Vybraná posloupnost|vybrané posloupnosti]], které obě mají různé limity.

## Příklady

---
>Hledejte limitu posloupnosti $\Large\{\frac{1}{n}\}_{n=1}^\infty$. Výsledek dokažte pomocí definice limity.
>
>*Když za $\Large\frac{1}{n}$ budeme dosazovat větší a větší číslo, tak bude vznikat menší a menší číslo, tudíž se bude zlomek víc a víc blížit k nule.*
>
>Pro libovolné $\large\varepsilon \gt 0$ platí, že $\large|a_n - a| \lt \varepsilon$.
>$$\large\begin{aligned}
>|a_n - a| &\lt \varepsilon \\
>|\frac{1}{n} - 0| &\lt \varepsilon \\
>|\frac{1}{n}| &\lt \varepsilon
>\end{aligned}$$
>Protože $\varepsilon$ bylo libovolné číslo větší než nula, tak $\Large\frac{1}{n}$ musí být menší nebo rovno nule. Vzhledem k tomu, že je zlomek v absolutní hodnotě, tak jediné vyhovující číslo je 0.

---

>Uveďtě výsledek limity $\large\lim_{n\to\infty}{\sqrt[n]{x}}$ pro $x \ge 0$.
>
>$$\large
>\lim_{n\to\infty}{\sqrt[n]{x}} = 
>\lim_{n\to\infty}{x^{\frac{1}{n}}} = 
>x^{\lim_{n\to\infty}{\frac{1}{n}}} =
>x^0 = 1
>$$