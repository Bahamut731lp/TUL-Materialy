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

## Derivace inverzní funkce
$$\large
\begin{aligned}
	y &= f(x) \\
	f'(x) &= \frac{1}{(f^{-1})'(y)}
\end{aligned}$$


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

## Derivace logaritmů
$$\large\begin{eqnarray}
(c^x)^\prime&=&c^x\ln c;\quad c>0\\\\
(e^x)^\prime&=&e^x\\\\
(\log_cx)^\prime&=&\frac{1}{x\cdot \ln c};\quad c>0\wedge c\ne0\\\\
(\ln x)^\prime&=&\frac{1}{x}
\\\\\\
\end{eqnarray}$$

$$\Large
\begin{aligned}

\frac{dx}{dy}\left(\frac{\sqrt{x}}{4-\sqrt{x}}\right) \\
\\
f &= \sqrt{x}\\
\frac{dx}{dy}(f) &= \frac{1}{2}x^{-\frac{1}{2}}=\frac{1}
{2\sqrt{x}}\\
\\
g &= 4 - \sqrt{x}\\
\frac{dx}{dy}(g) &= -\frac{1}{2\sqrt{x}} \\
\\
\frac{dx}{dy}\left(\frac{\sqrt{x}}{4-\sqrt{x}}\right) &= \frac{f'\cdot{g} - f\cdot{g'}}{g^2} \\
&= \frac{\frac{1}
{2\sqrt{x}}\cdot{(4 - \sqrt{x})} - \sqrt{x}\cdot\left({-\frac{1}
{2\sqrt{x}}}\right)}{(4 - \sqrt{x})^2} \\
&= \frac{\frac{\cancel{4}}
{\cancel{2}\sqrt{x}} - \frac{\cancel{\sqrt{x}}}{2\cancel{\sqrt{x}}}+{\frac{\cancel{\sqrt{x}}}
{2\cancel{\sqrt{x}}}}}{(4 - \sqrt{x})^2} \\

&= \frac{\frac{2}{\sqrt{x}}-\frac{1}{2}+\frac{1}{2}}{(4-\sqrt{x})^2} \\
&= \frac{2}{\sqrt{x}} \cdot \frac{1}{16 - 8\sqrt{x}+x}


\end{aligned}
$$