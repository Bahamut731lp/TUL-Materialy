# Derivace ve směru
>**TL,DR:**
>- Derivace ve směru je součin směrového vektoru a [[Gradient|gradientu]] funkce.

[[Parciální derivace]] nám říkají, jak se funkce mění ve směru nějaké osy - např. osy x, nebo osy y. Občas se nám ale hodí vědět, jaká je derivace v námi zkoumaném směru. K tomu slouží stejně pojmenované derivace ve směru, pro kterou si zavedeme nějaký směrový vektor $\vec{v}$, o $n$ složkách.

---
Uvažujme tedy například 
- vektor $\vec{v} = \begin{bmatrix}a \\ b\end{bmatrix}$ 
- a funkci $f(x,y)$, 
 
poté **derivací ve směru** myslíme součin prvků směrového vektoru a [[Gradient|gradientu]] funkce $f$.

>**Výpočet derivace ve směru za pomocí gradientu.**
>$$\Large\nabla_\vec{v}{f(x,y)} = a\cdot\frac{\partial{f}}{\partial{x}} + b\cdot\frac{\partial{f}}{\partial{y}}$$

Tento vztah platí díky geometrickému významu gradientu, kdy gradient jako takový ukazuje ve směru nejrychlejšího růstu funkce.

>**Výpočet derivace ve směru za pomocí formální definice**
>TODO: Limita

