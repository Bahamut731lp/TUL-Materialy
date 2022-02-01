# Zobrazení
Zobrazení je druhem [[Binární relace|binární relace]], která jednomu prvku (vzoru) přiřazuje **nejvýše jeden** prvek (obraz).

>Zobrazení nám tedy říká, jakým způsobem máme přiřadit věci z jedné skupiny k věcem z druhé skupiny.
> ![[Pasted image 20211011203657.png]]


Důležitou vlastností je, že můžeme přiřadit **nejvýše jeden** prvek. Nemůžeme se nám tedy stát, že by prvek z první skupiny "ukazoval" na více prvků ze skupiny druhé. Jak bychom pak věděli, na který máme koukat???

```mermaid
flowchart TB
	A[Obraz] -- tenhle? --> B[Vzor]
 	A -- nebo tenhle? --> C[Vzor]
```

## Druhy zobrazení
Podle toho, jakým způsobem jsou prvky výchozí množiny zobrazeny do cílové množiny se zobrazení dělí na:

---
Zobrazení **na množině**
- *Výchozí a cílová množina jsou totožné*
---
Zobrazení **množiny do množiny** 
- *Ke každému vzoru existuje právě jeden obraz. *
---
Zobrazení **množiny na množinu**
- *Každý obraz má svůj vzor*
- *Tzn. zobrazuje se na celou cílovou množinu*
---
Zobrazení množin se také dá dělit podle jejich vlastností na:

---
**Prosté zobrazení** <sup>(injektivní zobrazení)</sup>
- Každý vzor má jiný obraz
- Mohou existovat *obrazy* bez *vzoru*
```mermaid
flowchart TB

subgraph Vzory
A[Vzor 1]
B[Vzor 2]
C[Vzor 3]
end

subgraph Obrazy
K[Obraz 1]
L[Obraz 2]
M[Obraz 3]
N[Obraz 4]
end

A --> K
B --> L
C --> M
```

> $$f: A \rightarrow B$$
>$$
\forall[x_1,y_1],[x_2,y_2]
\in
f: x_1 \not= x_2 \implies y_1 \not= y_2
>$$
>"Pro každou uspořádanou dvojici platí, že obrazy nejsou stejné, ani vzory nejsou stejné." *<sub>(asi, pozn. red)</sub>*

---
**Vzájemně jednoznačné zobrazení** <sup>(bijektivní zobrazení)</sup>
- Každý vzor má svůj obraz
- Žádný prvek nezůstává nepřiřazený
```mermaid
flowchart TB

subgraph Vzory
A[Vzor 1]
B[Vzor 2]
C[Vzor 3]
D[Vzor 4]
end

subgraph Obrazy
K[Obraz 1]
L[Obraz 2]
M[Obraz 3]
N[Obraz 4]
end

A --> K
B --> L
C --> M
D --> N
```
> $$f: A\leftrightarrow B$$

---
**Inverzní zobrazení**
- Zobrazuje "opačným směrem" než původní zobrazení
	- Obrazům přiřazuje vzory
- Zobrazení musí být *prosté* zobrazení *na*

> $$ f(a) = b\leftrightarrow f^{-1}(b) = a  $$