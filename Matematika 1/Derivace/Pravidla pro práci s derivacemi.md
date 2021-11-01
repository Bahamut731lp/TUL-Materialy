# Základní pravidla a vzorce pro derivace
Pro práci s derivacema je vhodné znát pár vzorců a vztahů, které výpočty urychlují.

>**TL,DR:**
>- Derivace součtu a rozdílu: $\large(f(x) \pm g(x))' = f'(x) \pm g'(x)$

## Derivace součtu a rozdílu
$$\large\begin{aligned} 
(f(x)+g(x))' &= \lim_{x\to x_0} \frac{(f(x)+g(x)) - (f(x_0) + g(x_0))}{x-x_0} \\
&= \lim_{x\to x_0} \frac{f(x)+g(x) - f(x_0) - g(x_0)}{x-x_0} \\
&= \lim_{x\to x_0} \frac{f(x)-f(x_0)+g(x)- g(x_0)}{x-x_0} \\
&= \lim_{x\to x_0} \frac{f(x)-f(x_0)}{x-x_0} + \frac{g(x)- g(x_0)}{x-x_0} \\
&= \lim_{x\to x_0} \frac{f(x)-f(x_0)}{x-x_0} + \lim_{x\to x_0}\frac{g(x)- g(x_0)}{x-x_0} \\
&= f'(x) + g'(x)
\end{aligned}$$

Analogické odvození je i pro **derivaci rozdílu**.

$$\large (f(x)-g(x))' = ... = f'(x)-g'(x)$$

## Derivace součinu



## Standardní funkce
>Derivace konstatní funkce je 0
>$$\large c'=0$$

>Derivace lineární funkce je 1
>$$\large x'=1$$

>Derivace mocniné funkce
>$$\large (x^c)'=c\cdot x^{c-1}$$
>Např. $x^2=2x^1$

## Derivování operací

>$$\large	
>\begin{aligned}
>(f + g)' &= f' + g' \\
>(c \cdot f)' &= c \cdot f' \\
>(f \cdot g)' &= f' \cdot g + f \cdot g' \\
>\left(\frac{f}{g}\right)' &= \frac{f' \cdot g - f \cdot g'}{g^2}
>\end{aligned}$$

## Derivování inverzní funkce

>$$\large f(x_0)' = \frac{1}{(f^{-1}(y_0))'}$$