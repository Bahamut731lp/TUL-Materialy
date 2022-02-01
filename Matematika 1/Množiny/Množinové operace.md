# Množinové operace
[[Množiny]] používáme pro uchování různých prvků se společnými vlastnostmi - co kdybychom ale s množinou chtěl nějak manipulovat - např. pokud máme množinu výsledků měření a chceme odstranit chybná měření - jak na to? Odpovědí jsou **množinové operace**.

Množinové operace nám dovolují provádět operace jako "sčítání" a "odečítání" mezi dvěma množinami. Narozdíl od sčítání a odečítání čísel se ale tady trochu mění terminologie.

## Značení množinových operací
|Operace|Značení|
|:--:|:--:|
|Sjednocení|$A\cup{B}$|
|Průnik|$A\cap{B}$|
|Rozdíl|$A\setminus{B}$|
|Symetrický rozdíl|$A\triangle{B}$|
|Doplněk|$U\setminus{B}$|

---
## Sjednocení
Sjednocení množin (např. $A$ a $B$) vytvoří množinu, ve které **jsou všechny prvky vstupních množin**.

>$$A=\set{\color{lime}1,2,3}$$
>$$B=\set{\color{red}7,8,9}$$
>$$A\cup{B}=\set{\color{lime}1,2,3,\color{red}7,8,9}$$

![[Pasted image 20211013215239.png]]

---
## Průnik
Průnik množin (např. $A$ a $B$) vytvoří množinu, ve které **jsou pouze společné prvky vstupních množin**.

>$$A=\set{1,2,\color{red}3,4,5}$$
>$$B=\set{\color{red}3,4,5\color{white},6,7}$$
>$$A\cap{B}=\set{\color{red}3,4,5}$$

![[Pasted image 20211013214840.png]]

---
## Rozdíl

Rozdíl funguje podobně jako odečítání čísel - od první množiny (např. $A$) odečtene prvky druhé množiny (např. $B$).

>$$A=\set{1,2,3,4,5,6,7,8,9}$$
>$$B=\set{1,3,5,7,9}$$
>$$A\setminus{B}=\set{2,4,6,8}$$

![[Pasted image 20211013215724.png]]

Pár poznámek k rozdílu množin:
- Pokud odečteme dvě stejné množiny, výsledek bude opět prázdná množina
- Pokud odečteme prázdnou množinu, výsledkem bude množina, od které odečítáme ($A\setminus\emptyset=A$)

---
## Symetrický rozdíl
Symetrický rozdíl je kombinací rozdílu, sjednocení a průniku. Slovně můžeme číst, že od **sjednocení množin odečteme jejich průnik**.

Efektivně tak dostáváme prvky, které jsou jenom v jedné z množin.

>$$A=\set{\color{lime}1,2,\color{red}3,4,5}$$
>$$B=\set{\color{red}3,4,5,\color{lime}6,7}$$
>$$A\triangle{B}=A\cup{B}\setminus{A\cap{B}}=\set{\color{lime}1,2,6,7}$$

![[Pasted image 20211013221348.png]]

---
## Doplněk
Doplněk představuje všechny prvky, které nejsou v množině, na kterou doplněk používáme. Laicky by se dalo říct, že je to "všechno ostatní" či "všechno okolo".

Při dělání doplňku potřebujeme  vědět, v jaké [[Číselné množiny|číselné množině]] se vlsatně pohybujeme, protože doplněk bere v potaz i "okolní svět" množiny.
>$$A=\set{1,2,3,4,5}$$
>$$A'=\mathbb{R}\setminus{\set{1,2,3,4,5}}$$

Pokud je tedy naše okolí množina reálných čísel, tak doplněk množiny $A$ jsou všechna reálná čísla, kromě čísel $\set{1,2,3,4,5}$.

![[Pasted image 20211013215731.png]]


