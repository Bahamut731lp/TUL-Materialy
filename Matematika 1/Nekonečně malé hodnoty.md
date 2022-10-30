# Nekonečně malé hodnoty
Nekonečně hodnoty (odborně **Infinitezimální hodnoty**) jsou hodnoty s malým písmenem $d$ na začátku (např. $dx$, $dy$, $dz$, ...), které označují "trochu něčeho", např. 
- *trochu* $x$
- *trochu* $y$
- *trochu* $z$
- ...

V trochu formálnějším prostředí se říká, že to je
- *nekonečně malé $x$*
- *nekonečně malé $y$*
- *nekonečně malé $z$*
- ...

Jak malá je ale "nekonečně malá" hodnota? Záleží na kontextu. Představme si třeba hodiny - v porovnání s hodinami jsou minuty menší, ale sekundy ještě menší. A ještě menší jsou milisekundy, či mikrosekundy. Vždy záleží na úhlu pohledu, ze kterého pracujeme.

Vybraným hodnotám se pak konkrétněji v kontextu [[Úvod do derivací|derivací]] říká [[Diferenciál|diferenciál]]. 

## Kdy lze nekonečně malé hodnoty zanedbat
Podle toho, k čemu se tyto nekonečně malé hodnoty vážou, lze rozhodnout, zda jsou zanedbatelné, a nebo zda mají nějaký efekt, se kterým je potřeba počítat. 

|Příklad|Je zanedbatelná?|
|:--:|:--:|
|$x\cdot{dx}$|Ne|
|$x^2\cdot{dx}$|Ne|
|$a^x\cdot{dx}$|Ne|
|$dx\cdot{dx}$|Ano|

Ukažme to na příkladu - máme $x$, které reprezentuje nějakou kvantitu, která může po malých částech růst. Jako funkci bychom to mohli zapsat ve tvaru $x + dx$. Pokud bychom chtělo vytvořit čtverec, tak by rovnice vypadala takto

$$(x+dx)^2=x^2+2x\cdot{dx}+(dx)^2$$

Když si rozebereme jednotlivé členy, tak 
- $x^2$ je prostě kvadratický nárůst, nic nového.
- V druhém členu k tomu přičteme dvakrát původní kvantitu a ještě trochu té původní kvantity
- V třetím členu přičteme trošku z trocha původní kvantity.

Když se na to člověk podívá takhle, tak co tam udělá ten třetí člen? O jak moc změní trocha trošky? No o moc ne. To je tedy člen, který můžeme zanedbat.

> **TL,DR:** Nekonečně malé hodnoty nás vždycky zajímají toho nejnižšího řádu (takže s nejnižším exponentem), protože ty dělají největší rozdíl ve výsledku

