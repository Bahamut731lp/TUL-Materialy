Pole (anglicky **Array**) je [[Datový typ#Strukturovaný DT|strukturovaný datový typ]], který seskupuje pevný počet položek stejného typu.

>[!tldr]
>- Pole je skupina hodnot stejného [[Datový typ|datového typu]] o pevné délce
>- Prvky jsou rozlišovány pomocí indexů
>- Jeden index může ukazovat pouze na jednu položku (jsou jednoznačné)

Při definici pole určujeme jeho
- rozměr[^1]
- a [[Datový typ|datový typ]] prvků pole

Index pole je [[Datový typ#Jednoduchý DT|ordinální datový typ]] (nejčastěji `integer`), avšak může být indexován např. i řetězcem (pak se jedná o [[Tabulka|ADT tabulka]]).

## Dynamická pole
Dynamické pole je [[Abstraktní datový typ|kontejner]] nad polem, který odstraňuje omezení fixní velikosti pole.

>[!info] Princip dynamického pole
>Jednotlivé prvky jsou ukládány ve vnitřním poli. 
>- Jakmile je jeho kapacita naplněna, tak se alokuje nové a větší pole[^2]
>- Pokud dlouho zůstává neobsazené, alokuje se menší pole

[^1]: Rozměr pole určuje, kolik prvků se do daného pole vejde, zároveň slouží pro správně předalokování paměti.
[^2]: Zpravidla se volí dvakrát větší velikost kvůli [[Amortizovaná složitost|amortizaci]]