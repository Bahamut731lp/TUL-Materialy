# Frobeniova věta
Frobeniova věta říká, za jakých podmínek má soustava lineárních rovnic řešení.

>**TL,DR:**


Frobeniova věta slouží jako propojení [[Matice|matic]] a [[Lineární zobrazení|lineárního zobrazení]], jelikož každé lineární zobrazení lze reprezentovat maticově a naopak, každá matice představuje nějaké lineární zobrazení.

Pro názornost to vezmeme z obou konců.

---
## Definice z pohledu matic
Frobeniova věta říká, že soustava lineárních rovnic má řešení, pokud se [[Hodnost matice|hodnost matice]] soustavy rovná [[Hodnost matice|hodnosti]] [[Rozšířená matice|rozšířené matice]] soustavy.

Znamená to, že matice levé strany rovnic musí mít stejnou hodnost jako matice pravé strany rovnic. Ještě jinak řečeno, musí mít stejně nenulových řádků.

>Matice
>$$\begin{bmatrix}
>1 & 2 &\bigm| & 3 \\
>5 & 8 &\bigm| & 4 \\
>\end{bmatrix}$$
>Má řešení, protože se hodnost levé strany $h(M_L)$ rovná hodnosti matice pravé strany $h(M_P)$

>Matice
>$$\begin{bmatrix}
>3 & 9 &\bigm| & 7 \\
>45 & 15 &\bigm| & 5 \\
>0 & 0 &\bigm| & 0 \\
>\end{bmatrix}$$
>Má řešení, protože se opět hodnosti rovnají

>Ale matice
>$$\begin{bmatrix}
>3 & 9 &\bigm| & 7 \\
>45 & 15 &\bigm| & 5 \\
>0 & 0 &\bigm| & 7 \\
>\end{bmatrix}$$
>Nemá řešení, protože se hodnosti se nerovnají
>
>$$\begin{aligned}
>h(M_L)&= 2 \\
>h(M_P)&=3 \\
>2 \not=3 &\implies h(M_L) \not= h(M_P)
>\end{aligned}$$

---
## Definice z pohledu lineárního zobrazení
Je-li $L$ [[Lineární zobrazení|lineární zobrazení]]
- z prostoru $U(M, \oplus, \otimes)$
- do prostoru $V(N, \oplus, \otimes)$

a dán vektor $b$ z prostoru obrazů (prostor $V$), tak platí, že
- Řešení existuje, náleží-li vektor $b$ do oboru hodnot zobrazení $L$
- Pokud řešení existuje a náleží do prostoru vzorů, pak mohou existovat i další vzory
- Další vzory musí splňovat to, že se dají vyjádřit jako vektorový součet původního vzoru a vektoru z [[Jádro zobrazení|jádra zobrazení]] $L$.

prvek $b$, který náleží do množiny obrazů ($b \in N$), poté můžeme hledat takové vzory, které se zobrazí právě do prvku $b$.

---
## Jak spolu tyto definice souvisí
*Doplnit později*