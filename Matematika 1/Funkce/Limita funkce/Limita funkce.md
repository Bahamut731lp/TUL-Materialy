# Limita funkce
Limity jsou nástrojem pro úvahu, jak se funkce chová v nějakém pro nás zajímavém bodě. Dovolují nám totiž zjistit, jaká funční hodnota by se mohla v daném bodě nacházet bez potřeby toho, že musí být funkce v bodě definována. 

Limity slouží jako základ pro [[Úvod do derivací|derivaci]] a [[Úvod do integrace|integraci]].

> TL,DR:
> - Limity říkají, jakou hodnotu by měla funkce, kdybychom se nekonečně blízko přibližovali ke zkoumanému bodu
> - Můžeme se přibližovat z jedné strany (zleva a zprava) a nebo z obou stran, podle toho dělíme limity na **jednostranné** a **oboustranné**.
> - Aby existovala oboustranná limita, musí mít jednostranné limity z obou stran stejnou hodnotu.
> - Limity můžeme aproximovat pomocí grafu či tabulky hodnot

---
## Jednostranná limita
Jednostranná limita je taková limita, ve které se ke zkoumanému bodu přibližujeme nekonečně blízko pouze z jedné strany - buďto **zleva** nebo **zprava**.

$$\large\begin{cases}
\lim_{x \to c^+} f(x) &\text{Značení limity zprava} \\
\lim_{x \to c^-} f(x) &\text{Značení limity zleva}
\end{cases}$$
V zápisu poznáme, jestli se jedná o jednostrannou limitu tím, že u zkoumaného bodu bude malé + nebo -. Jestliže tam žádné znaménko není, jedná se o [[#Oboustranná limita|oboustrannou limitu]].

Limita zleva je tedy hodnota funkce v nějakém bodě, když se k němu blížíme nekonečně blízko **z levé strany směrem doprava**. Naopak limita zprava je případ, kdy se blížíme nekonečně blízko k bodu **z pravé strany směrem doleva**.

> Když se k něčemu blížíme nekonečně blízko, říkáme, že se k tomu blížíme limitně. Tento způsob vyjádření používáme hlavně, když mluvíme o nevlastních limitách.
> 
> *Např.: Funkce $f$ se v nekonečnu limitně blíží k nule.*

## Oboustranná limita
Oboustranná limita[^1] je taková limita, u které se funkce zleva a zprava blíží ke stejnému bodu, tj. **limita zprava** a **limita zleva** mají **stejnou hodnotu**.

$$\Large
\begin{aligned}
	\lim_{ x \to {c^+} } {f(x)} &= A \\
	\lim_{ x \to {c^-} } {f(x)} &= A \\
	\lim_{x\to{c}}{f(x)} &= A
\end{aligned}
$$
---
##  Aproximace limity
Pokud by přímé vyhodnocení limity nebylo možné, či by tomu bránily jiné okolnosti, lze ji v rozumné míře odhadnout. Odhadnout ji můžeme buďto z **grafu funkce**, nebo trochu přesněji z **tabulky funkčních hodnot** v [[Okolí bodu|okolí]] zkoumaného bodu.

### Pomocí grafu
Graf funkce je skvělým nástrojem, který nám pomáhá **odhadnout** konečnou funkční hodnotu v nekonečně malém okolí.

### Pomocí tabulky
Občas máme pod rukama složitou funkci, u které by bylo složité si jí představit či nakreslit graf. Pokud ale máme k dispozici kalkulačku, můžeme limitu aproximovat pomocí **tabulky**, ve které si vypočítáme hodnoty "nekonečně blízko" k limitnímu bodu a následně vytvoříme rozumný odhad.

> Příklad: Vypočtete následující limitu
> $$\large\lim_{x\to{3}}\frac{x^3-3x^2}{5x-15}$$

Tuto limitu budeme aproximovat pomocí tabulky, kdy si rozepíšeme bližší a bližší hodnoty z obou stran a limitu v nich vyhodnotíme.

|x|$\Large\frac{x^3-3x^2}{5x-15}$||x|$\Large\frac{x^3-3x^2}{5x-15}$|
|:--:|:--:|:--:|:--:|:--:|
|2,9|1,682||3,1|1,991|
|2,99|1,788||3,01|1,812|
|2,999|1,7988||3,001|1,801|

Z tabulky můžeme usoudit, že limita když se $x$ blíží 3 by mohla být 1,8.
$$\large\lim_{x\to{3}}\frac{x^3-3x^2}{5x-15} \approx 1,8$$
---
## Formální definice limity
Limity byly doteď popisovány tak nějak pro uchopení konceptu a geometrického významu. Doteď jsme ale dokázali limity v zajímavých bodem maximálně aproximovat, což je sice pěkné, ale je zde potenciál pro získání přesnějších výsledků.

>Tvrzení: $\lim_{x \to c} f(x) = L$
>
*Funkční hodnotu $f(x)$ můžeme dostat "libovolně blízko" k bodu $L$ tím, že proměnnou $x$ dostatečně přiblížíme k bodu $c$*

Tohle tvrzení nám říká, že pokud na ose y existuje [[Okolí bodu|okolí bodu]] $L$ (pojmenujeme ho např. okolí *epsilon*), tak také existuje okolí bodu $c$ na ose x (pojmenujeme ho např. okolí *delta*), ve kterém funkční hodnoty bodů z okolí *delta* spadají do okolí *epsilon*.

>**Definice vlastní limity funkce:**
>Funkce $f$ má vlastní limitu $A$ v bodě $c$, pokud existuje $\delta$-okolí bodu $c$ takové, že všechny $x$ z $\delta$-okolí mají funkční hodnotu v $\varepsilon$-okolí.

[^1]: Běžně se oboustranné limitě říká prostě *limita*