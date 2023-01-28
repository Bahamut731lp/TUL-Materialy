Datový typ (dále jen *DT*) je název pro [[Množiny|množinu]] hodnot a [[Množiny|množinu]] operací, které jde nad danými hodnotami provádět.

>[!tldr]
>- Datový typ definuje, co může mít za hodnoty, a co za operace s nima můžem dělat


## Prázdný DT
Prázdný [[Datový typ|datový typ]] (`void`) je takový typ, který nemá žádné hodnoty a nelze s nim provádět žádné operace.

Nejčastěji se využívá pro označení [[Procedury|procedur]].

## Jednoduchý DT
Jednoduchý [[Datový typ|datový typ]] je takový typ, který v paměti ukládá data přímo.

> [!info] Ordinální datový typ
Ordinální datové typy jsou takové typy, které lze zobrazit na množině celých čísel
>- Mají jasně určeného předchůdce a následovníka
>- Pozici hodnoty lze ohodnotit ordinálním číslem
>>[!example] Ordinální typ `enum`
>>- Jednotlivé hodnoty mají přiřazené ordinální číslo
>>```c
>>enum DNY {
>>	PONDELI,
>>	UTERY,
>>	STREDA,
>>	CTVRTEK
>>}
>>```

> [!info] Neordinální datový typ
> Neordinální datové typy jasné sousedy nemají. 
> - Mezi takové typy např. patří *real*.

## Strukturovaný DT
Strukturovaný [[Datový typ|datový typ]] je takový typ, který seskupuje [[#Jednoduchý DT|jednoduché datové typy]]. Tyto DT poskytují prostředky pro práci s jednotlivými prvky.

> [!info] Pole
> viz [[Algoritmizace a datové struktury/Strukturované datové typy/Pole]]


## Abstraktní DT
viz [[Abstraktní datový typ]]