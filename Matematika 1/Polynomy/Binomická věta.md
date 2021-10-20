# Binomická věta
Jedná se o zobecnění známých vzorečků pro rozklad zárovek jako je $(a+b)^2$

>Formální zápis binomické věty:
>$$
>(a+b)^n=
>\textcolor{red}{\sum^n_{k=0}}
>\textcolor{yellow}{n \choose k}
>\textcolor{orange}{a^{n-k}b^k}$$
>$$a, b \in \mathbb{R}$$
>$$n \in \mathbb{N}$$

*Vysvětlení*: Rozklad získáme tím, že 
- budeme počítat [[Sumace|sumu]]
	- od $k$ (což je 0)
	- do $n$ ("na kolikátou" závorku umocňuji)
- suma se skládá ze dvou věcí
	- ze <span style="color: yellow">členu binomického rozvoje</span>
	- a z <span style="color: orange">proměnných s patřičnými exponenty</span>

Jak ale spočítat člen binomického rozvoje? K tomu je možná dobrý si říct, co to vůbec binomický [[Rozvoj|rozvoj]] je.

## Binomický rozvoj
Binomický rozvoj je to, čemu se říká po rozkladu vzorečku $(a+b)^n$.

>$$(a+b)^2=\textcolor{cyan}{a^2+2ab+b^2}$$
> <span style="color: cyan">Pravá strana</span> rovnice je **binomický rozvoj**, jelikož jsme výraz rozvinuli ze zkráceného tvaru...

Asi by to ale chtělo nějak šikovně vypočítat koeficienty jednotlivých proměnných, ne? K tomu nám může pomoct [[Pascalův Trojúhelník]], který nám pomáhá určit **koeficienty binomického rozvoje** - to jsou čísla před jednotlivými členy rozkladu.


