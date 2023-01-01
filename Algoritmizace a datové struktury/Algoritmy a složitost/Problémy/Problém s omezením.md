**Problémy s omezením** jsou problémy, ve kterých hledáme takové řešení, které uspokokuje všechny omezení kladená na vstupní data.

>[!tldr]
>- Problémy s omezením hledají takové řešení, které uspokokuje všechna integritní omezení
>- Nejjednoduším algoritmem pro jejich řešení je [[Backtracking|backtracking]].


- Množinu proměnných, které mají neprázdný [[Definiční obor|definiční obor]]
- Množinu omezení

## Množina omezení
Množina omezení představuje sadu vztahů, které ukládají omezení na jednotlivé proměnné.
>[!example]+ Příklady omezení
>Mezi taková omezení patří například
>- Že proměnná musí být větší než konstanta ($x_i > 3$)
>- Že proměnná musí být menší než jiná konstanta

Tato omezení poté dělíme na [[Unární relace|unární omezení]] a [[Binární relace|binární omezení]]. 
- Unární omezení obsahuje jednu proměnnou (např. $x > 3$), 
- zatímco binární potřebuje proměnné dvě (např. $x > y$)

Unární omezení lze aplikovat před 