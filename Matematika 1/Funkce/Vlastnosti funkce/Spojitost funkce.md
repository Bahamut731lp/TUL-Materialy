# Spojistost funkce
Funkce je spojitá, pokud se její hodnoty mění plynule.

>**TL,DR:**


## Cauchyho definice
Přesnější definicí je takzvaná **Cauchyho definice**, která říká:

>O funkci $f$ řekneme, že je spojitá **v bodě c**, pokud pro kladné číslo $\large \varepsilon$ existuje kladné číslo $\large\delta$ tak, že platí vztahy:
>$$\Large\begin{aligned}
>|f(x) - f(c)| &< \varepsilon \\
>\forall x &\in (c-\delta, c+\delta)
\end{aligned}$$
>![[Spojitost funkce - Cauchyho definice.png]]

Pojďme tu hnusnou definici rozebrat - funkce je spojitá v bodě c
- pokud po zvolení nějakého kladného čísla (<span style="color:red">číslo $\large \varepsilon$</span>)
- pro něj najdeme odpovídající číslo (<span style="color:lime">číslo $\large \delta$</span>)
- pomocí vztahů $|f(x)-f(c) < \varepsilon|$ a $|x-c|<\delta$.

Z obrázku výše jde vidět, že se pomocí čísel <span style="color:red">$\large \varepsilon$</span> a <span style="color:lime">$\large \delta$</span> vytváří nějaká [[Okolí bodu|okolí bodu]]. To je proto, abychom mohli zkoumat
- Spojitost zleva
- a spojitost zprava

Pokud tedy nerovnost funkčních hodnot ($|f(x) - f(c)| < \varepsilon$) platí jenom "na jedné straně", tak je z toho směru spojitá.
- $\large x\in\left<{x,x+\delta}\right) \implies$ Pro všechna $\large{x}$ **z pravého [[Okolí bodu|okolí]]** je funkce spojitá
- $\large x\in\left({x-\delta,x}\right> \implies$ Pro všechna $\large{x}$ **z levého [[Okolí bodu|okolí]]** je funkce spojitá

Tohle můžeme vidět i na obrázku u definice. Od té tučné zelené čáry, která nám značí proměnnou $\large{x}$, máme dvě části - jednu "nalevo" a druhou "napravo" - a my právě dokážeme říct, v které z nich je funkce spojitá, a v které ne.

Ty dva vzorečky v podstatě říkají, že když si zvolímě nějaké okolí, tak pro každé $x$ (pro každý argument funkce) musí být nějaká funkční hodnota.

Když se podíváte na ty [[Intervaly|intervaly]] výše o spojitosti z pravého nebo levého okolí, tak jsou polootevřené.  To znamená, že námi zkoumaný bod $\large{x}$ **musí** být ve funkci definovaný alespoň z jedné strany. Pokud je funkce spojitá z obou stran, tak říkáme, že je funkce v bodě spojitá.

## Spojitost a složené funkce
Spojitost se při skládání funkcí přenáší. 

Pokud bychom prováděli aritmetické operace s funkcemi $\large{f}$ a $\large{g}$, které jsou obě spojité v nějakém vybraném bodě (např. $\large{c}$), tak poté jejich
- Absolutní hodnoty (${|f|, |g|}$)
- Součet ($f+g$)
- Rozdíl ($f-g$)
- Součin ($f\cdot g$)
- a podíl, když funkce v jmenovateli není rovna nule ($\frac{f}{g}, g(c)\not= 0$)
- **budou také spojité ve vybraném bodě**

Obdobně to platí pro složené funkce - $f(g)$ bude spojitá, pokud jsou obě funkce ve vybraném bodě spojité