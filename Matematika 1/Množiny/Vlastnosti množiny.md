# Množiny
Množina je **soubor určitých prvků** se společnou vlastností. Běžně je značíme velkými písmeny ($M, N, P, ...$) a jejich prvky písmeny malými - podobně jako u [[Matice|matic]].

Množiny můžeme definovat buďto
- výčtem $M=\set{1,2,3,4,5,...}$
- nebo vlastností $M=\set{x\in M, x< 4}$

Množiny tedy používáme k vymezení možností, ze kterých můžeme vybírat. Často potřebujeme vyjádřit, jestli něco do množiny
- **patří** ($1\in M$)
	- *Jednička patří/náleží do množiny $M$)*
- nebo **nepatří** ($1 \not\in M$)
	- *Jednička nepatří/nenáleží do množiny $M$*

---
## Vlastnosti množin
### Prázdné množiny
Množiny mají speciální vlastnost - a to, že mohou být prázdné. Prázdné množiny se značí $M=\set{}$ nebo $M=\emptyset$.
- Pozor, $M=\set{\emptyset}$ je **množina s prázdnou množinou uvnitř** a není tím pádem prázdná!

---
### (Ne)uspořádanost prvků
V množinách na pořadí prvků **nezáleží**
>$$M=\set{1,2,3}$$
$$N=\set{3,1,2}$$

Množiny $M$ a $N$ jsou v tomto případě **stejné**.

---
### Duplicity
Množinám ani nevadí několikanásobný výskyt jednoho a toho samého prvku.
>$$M=\set{1,2,3,4,5}$$
$$N=\set{3,5,5,1,2,5,4}$$

Tyto množiny jsou **také stejné**. *"Ale však množina $N$ má více prvků!" vás slyším zvolat.* - Odpověď je v další části.

Pokud množina nemá duplicity, tak se jí říká **prostá množina**, pokud duplicity má, občas se jí říká **kolekce**. Je to ale čistě jenom jiná terminologie, pořád to jsou **množiny**.

---
### Velikost množiny
Při počítání velikosti množiny **nebereme v potaz duplicitní výskyty** - jinak řečeno, **počítáme pouze unikátní prvky**.

>$$\set{1,2,3}=\set{1,2,3}$$
>$$\set{1,2,3}=\set{3,1,2}$$
>$$\set{a,b,c}=\set{a,a,b,c,b}$$
>$$\set{1,3,5,9}\not=\set{1,3,9}$$
>$$\emptyset\not=\set{x}$$

Množiny se tedy rovnají, pokud mají stejné prvky.

---
### Mohutnost množiny
Podle počtu prvků se určují **mohutnosti množiny**. 
- Množina **konečná** má konečný počet prvků
- Množina **nekonečná** má nekonečně mnoho prvků
- Množina **spočetná** jsou nekonečné množiny, jejichž prvky jsou označitelné přirozenými čísly
	- Všechny tedy mají shodný počet prvků
	- Např. celá čísla, celá kladná (přirozená), racionální čísla, ...

---
### Vnořování množin
Jako prvky množiny mohou být další množiny, přičemž se počítají **jako jeden prvek**.

>$$M=\set{1,\set{2},\set{3,\set{4,5}}, 6}$$


>$$M_1=1$$
>$$M_2=\set{2}$$
>$$M_3=\set{3,\set{4,5}}$$
>$$M_4=6$$

[^1]: Kdyby měli velikost větší, nazývala by se **nadmnožinou**, přičemž ta naše původní množina by byla podmnožinou.