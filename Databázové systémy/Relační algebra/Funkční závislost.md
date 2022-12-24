**Funkční závislost** popisuje vztah mezi [[Atribut|atributy]] v [[Relace|relaci]] a určuje jejich integritní omezení.

Pokud máme relaci $R(A,B)$, kde $A$ a $B$ jsou nějaké atributy, pak funkční závislost $A\to B$ znamená, že:
- $A$ jednoznačně určuje $B$
- $B$ je funkčně závislé na $A$

Jinak řečeno, když máme několik řádků tabulky, tak pokud má $A$ stejnou hodnotu, musí mít $B$ vždy také stejnou hodnotu.

Při vytváření funkčních závislostí se vyplatí ptát otázkou: "Co jednoznačně určuje další atributy?"

> Např. v případě rodného čísla můžeme říct, že rodné číslo jednoznačně určuje jméno a příjmení. Nemůže se nám totiž stát, že stejné rodné číslo bude mít dvě různá jména.

## Armstrongova pravidla (axiómy)
