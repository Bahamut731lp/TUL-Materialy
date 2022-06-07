# Booleovský výraz
Výraz představující logickou funkci. Každou funkce lze popsat několika ekvivalentními výrazy.

|Termín|Popis|
|:--|:--|
|**Term**|Výraz tvořený pouze proměnnými v log. součtu nebo součinu|
|**P-Term**|Term pouze s operací součinu|
|**S-Term**|Term pouze s operací součtu|
|**Minterm**|P-Term obsahující všechny nezávislé proměnné|
|**Maxterm**|S-Term obsahující všechny nezávislé proměnné|

>**Rozdělení termů:**
>
>![[terms.drawio.png]]


**Každou logickou funkci lze vyjádřit jako součet mintermů, nebo součin maxtermů.**

## Formy zápisu výrazu

|Zkratka|Forma|Vysvětlení|
|:--:|:--:|:--:|
|UNDF|Úplná normální disjunktní|Výraz tvořen součtem všech mintermů|
|UNKF|Úplná normální konjuktivní|Výraz tvořen součinem všech maxtermů|
