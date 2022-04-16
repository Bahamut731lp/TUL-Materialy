# Kvadratická forma



>**Formální definice kvadratické formy funkce**
>$$\Large Q(x) = \sum_{i = 1}^{n}a_{ii}x_{i}^2 + 2\sum_{i = 1}^{n}\sum_{j = 1}^{i - 1}a_{ij}x_{i}x_{j}$$
První suma bere diagonální členy matice, druhý člen bere prvky pod diagonálou, a protože je matice symetrická, vezmou se dvakrát.


Kvadratickou formu lze reprezentovat pomocí [[Matice|matice]],

$$\Large
\begin{bmatrix}
a & b & c \\ 
d & e & f \\ 
g & h & i
\end{bmatrix}$$

## Definitiní formy
|Název formy|Podmínka|
|--:|:--|
|Pozitivně definitní|$Q(x) \gt 0, \forall x \not= [0, ..., 0]$|
|Pozitivně semidefinitní|$Q(x) \ge 0, \exists x \not= [0, ..., 0]$|
|Negativně definitní|$Q(x) \lt 0, \forall x \not= [0, ..., 0]$|
|Pozitivně semidefinitní|$Q(x) \le 0, \exists x \not= [0, ..., 0]$|
|Indefinitní|Pokud nenastala jedna z předchozích možností|

## Příklady

>$\large Q(x, y) = x^2 + y^2$
>Forma je pozitivně definitní, protože kromě počátku jsou všechny funkcní hodnoty kladné.

>$\large Q(x, y, z) = x^2 + y^2$
>Forma je pozitivně semidefinitní, protože počátek je sice v počátku $[0, 0, 0]$, ale po dosazení bodu $[0, 0, z]$ je funkční hodnota taky nulová, nerovnost tedy není ostrá.
