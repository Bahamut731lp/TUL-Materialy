Komparační AD převodníky slouží k převodu [[Signál#Analogový signál|analogového signálu]] na [[Signál#Číslicový signál|číslicový (digitální) signál]]. Třída komparačních převodníků k tomu využívá tzv. [[Komparátor|komparátory]], které porovnávají vstupní napětí s referenčním napětím.

## Komparační paralelní
**Komparační paralelní AD převodník** využívá paralelně zapojených [[Komparátor|komparátorů]], ve kterých se porovnává vstupní napětí s referenční hodnotou z [[Dělič napětí|odporového děliče]].

Díky jednoduchosti obvodu je převod velmi rychlý, navíc se dá navzorkovat celé binární slovo najednou. Obrovskou *(pun inteded)* nevýhodou je, že je konstrukčně náročný. Na převod $N$ bitů je potřeba $2^{N-1}$ komparátorů. 

> **Ukázkové zapojení komparačního paralelního AD převodníku**
> 
> ![[Pasted image 20221130112350.png]]

## Komparační s postupnou komparací
**Komparační AD převodník s postupnou komparací** je převodník, který pro převod využívá principu [[Divide And Conquer]]. Nevýhoda [[#Komparační paralelní|paralelního komparačního převodníku]] byla ta, že se stává konstrukčně složitým na vyšším počtu bitů. Převodníky s postupnou komparací, jak už název napovídá, řeší tím, že převod rozdělí na menší "podpřevody", které postupně zpracovávají.

Výhodou tohoto přístupu je, že relativně zachováme rychlost převodu, zatímco zmenšíme počet komparátorů.

>**Schéma zapojení 8 bitového komparačního AD převodníku s postupnou komparací**
>
>![[Pasted image 20221130113206.png]]
>První AD převodník vytvoří horní 4 bity, které se
>- Pošlou na výstup
>- Použijí jako menšitel v rozdílovém zesilovači
>
>V rozdílovém zesilovači se vezme původní vstupní signál, a odečte se od něj analogová reprezentace 4 horních bitů. Tím získáme napětí, které reprezentuje pouze spodní 4 bity. Toto napětí zesílíme a následně převedeme. Výsledek převodu je spojení obou výsledků z obou převodníků