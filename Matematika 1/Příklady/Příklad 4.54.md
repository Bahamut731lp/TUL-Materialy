> [!example] Spočtěte obsah obrazce
> ohraničeného funkcí $x^2$ a přímkou procházející body $[−1, 1]$ a $[1,5]$

>[!help] Jak určit předpis přímky ze dvou bodů?
>viz [[Směrnicový tvar přímky#Určení ze dvou bodů]]

$$\Large\begin{aligned}
 f(x) &= x^2 && f(x)=0 \text{\;pro\;} x=0\\ 
 g(x) &= 2x+3 && g(x) = 0 \text{\;pro\;} x = \large-\frac{3}{2}
\end{aligned}$$

>[!info] Vypočítání [[Integrační meze|integračních mezí]]
>$$\Large
>\begin{aligned}
>	f(x) &= g(x) \\
>	x^2 &= 2x+3 \\
>	x^2-2x-3&=0 \\
>	(x-3)\cdot(x+1) &= 0 \\
>	x &\in\boxed{\set{-1, 3}}
>\end{aligned}
>$$

>[!info] Jak správně zapsat oblast mezi funkcemi?
>Nejprve zjistíme, která funkce je "výš" než ta druhá.
>
>Protože se funkce protínají akorát v bodech $x=-1$ a $x = 3$, tak je na tomhle intervalu ($x\in(-1,3)$) buďto **pod** nebo **nad** přímkou. Vezmem tedy $x$ z intervalu a dosadíme.
>$$\Large
>\begin{aligned}
>x &= 0 \\
>f(0) &= 0 \\
>g(0) &= 3 \\
>\end{aligned}$$
>
> Lze vidět, že bod na přímce má vyšší funkční hodnotu než bod na parabole. Oblast mezi nimi je tedy vyjádřena jako rozdíl mezi oblastí pod přímkou a oblastí pod parabolou: $\int{g(x)-f(x)}dx$


$$\Large
\begin{aligned}
	\int_{-1}^{3} g(x) - f(x)\;dx
\end{aligned}
$$



