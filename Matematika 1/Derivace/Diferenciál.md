# Diferenciál
Diferenciál je vyjádření změny [[Úvod do funkcí#Základní pojmy k funkcím|funkční hodnoty]] na a argumentu pomocí přímé úměrnosti.

>**TL,DR:**
>- Diferenciál funkce $f$ v bodě $a$ je $f'(a)h$

Funkce má tedy v bodě diferenciál, pokud jde její přírustek vyjádřit jako
>$$\large\Delta{f(a,h)}=f(a+h)-f(a)$$
>- $a$ je argument funkce
>- $h$ je přírustek, který chceme diferenciálem vyjádřit
>
>$$\large\Delta{f(a,h)}=A\cdot{h}+r(h)\cdot{h}$$
>- Další způsob zápisu diferenciálu
>- $A$ je konstanta, která je rovna derivaci funkce v bodě $a$ ($A = f'(a)$)
>- $r$ je funkce limitně se blížící k nule ($\lim_{h\to0}r(h) = 0$)

Funkce má v bodě diferenciál jenom tehdy, pokud v něm má i [[Úvod do derivací#Vlastní a nevlastní derivace|vlastní derivaci]].
- Existuje diferenciál $\iff$ Existuje derivace

## Značení
Výraz $f'(a)h$ - [[Úvod do derivací|derivaci]] v bodě $a$ krát okolí $h$ značíme pomocí. 

Pro značení se tedy používá $df(a)$, tedy **diferenciál** ($d$) funkce v bodě a ($f(a)$). Vzhledem k tomu, že to je diferenciál funkční hodnoty, tak se také značí jako $dy$

> Znázornění jednotlivých prvků diferenciálu funkce $f$ v bodě $c$:
> 
> ![[Pasted image 20211101011046.png]]

 ## Jaký je rozdíl mezi diferenciálem a derivací?
 Možná jste si všimli, že diferenciál vypadá fakt hodně jako derivace. Je mezi nimi vůbec nějaký rozdíl? No, kdyby nebyl, tak by se nezaváděli dva různé termíny, že.
 
 - **Derivace** vyjadřuje míru změny hodnot, aneb "jak rychle se něco mění"
 - **Diferenciál** vyjadřuje samotnou změnu hodnot

Z obrázku výše to jde i krásně vidět 
- Červená [[Tečna|tečna]] je **[[Úvod do derivací|derivace]]** funkce $f$
- **Diferenciál** je složen ze dvou komponent 
	- $\large Ah$
	- $\large r(h)h$
	- dohromady dávající rozdíl mezi funkčími hodnotami ($f(c+h)-f(c)$)

Derivaci můžeme vyjádřit jako poměr dvou diferenciálů:
- Diferenciálu funkce ($dy$)
- a diferenciálu proměnné ($dx$)
- $\large f'(x)=\frac{dy}{dx}$