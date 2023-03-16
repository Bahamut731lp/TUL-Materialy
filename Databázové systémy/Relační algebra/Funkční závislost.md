**Funkční závislost** popisuje vztah, resp. [[Zobrazení|zobrazení]], mezi [[Relační datový model|atributy]] v [[Relační datový model|relaci]] a určuje jejich integritní omezení.

>[!tldr]
>- Funkční závislosti zobecňují koncept [[Klíče|klíče]]
>- 

>[!example] Příklad
>Pokud máme relaci $R(A,B)$, kde $A$ a $B$ jsou nějaké atributy, pak funkční závislost $A\to B$ znamená, že:
>- $A$ jednoznačně určuje $B$
>- $B$ je funkčně závislé na $A$

Jinak řečeno, když máme několik řádků tabulky, tak pokud má $A$ stejnou hodnotu, musí mít $B$ vždy také stejnou hodnotu.

>[!tip] 
>Při vytváření funkčních závislostí se vyplatí ptát otázkou: 
>***Co jednoznačně určuje další atributy?***
>> [!example] Příklad
> >Např. v případě rodného čísla můžeme říct, že rodné číslo jednoznačně určuje jméno a příjmení. 
> >
> >Nemůže se nám totiž stát, že stejné rodné číslo bude mít dvě různá jména.

## Armstrongova pravidla (axiómy)
**Armstrongova pravidla** slouží k odvozování dalších [[Funkční závislost|funkčních závislostí]] z již dané množiny [[Funkční závislost|funkčních závislostí]].

>[!tip] 
>Jedná se rádoby o stejný proces, jak je tvorba [[Lineární obal|lineárního obalu]] z [[Báze|báze vektorového prostoru]]

>[!info] Axiomy
>>[!info] [[Dekompozice]]
>>Pokud $A \to b,c,d$, poté platí:
>>- $A \to b$
>>- $A \to c$
>>- $A \to d$
>
>>[!info] Sjednocení
>>Pokud platí $A \to b$, $A \to c$ a $A \to d$, poté platí:
>>- $A \to b,c,d$
>
>>[!info] Rozšíření
>>Pokud platí $A \to B$, poté platí:
>>- $AZ \to  BZ$
>
>>[!info] [[Tranzitivnost|Tranzitivita]]
>>Pokud platí $A \to B$ a $B \to C$, poté platí:
>>- $A \to C$
