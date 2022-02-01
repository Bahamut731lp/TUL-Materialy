# Omezení množiny
Pokud má množina:
- **horní mez**, nazývá se **shora omezená**.
- **dolní mez**, nazývá se **zdola omezená**.
- **horní i dolní mez**, nazývá se **omezená**.

## Meze
**Co je horní mez?**
Horní mezí označujeme číslo, které je větší nebo rovno všem prvkům množiny.

>$$\Large\begin{eqnarray} 
h &\in\mathbb{R}\\
\forall{x} &\in M\\
x &\le h
\end{eqnarray}$$
>Číslo $h$ z reálných čísel, pro který platí, že každé číslo $x$ z množiny $M$ je větší nebo rovno číslu $h$, nazýváme **horní mez** množiny $M$. 

**Co je dolní mez?**
Dolní mezí označujeme číslo, které je větší nebo rovno všem prvkům množiny.

>$$\Large\begin{eqnarray} 
d &\in\mathbb{R}\\
\forall{x} &\in M\\
x &\ge d
\end{eqnarray}$$
>Číslo $h$ z reálných čísel, pro který platí, že každé číslo $x$ z množiny $M$ je větší nebo rovno číslu $h$, nazýváme **horní mez** množiny $M$. 

## Supremum a infimum
Ze vztahu pro horní i dolní mez je vidět, že to jsou **všechna** čísla větší/menší než prvky množiny. Nás ale zajímají jenom takové meze, které bezprostředně omezují množinum, tj. které "stojí hned na kraji množiny". Z tohoto důvodu se zavedlo **supremum** a **infimum**.

**Supremum** = Nejmenší horní mez.
**Infimum** = Největší horní mez.

> **Věta o supremu a infimu**
> Pro každou [[Množiny#Druhy množin|neprázdnou množinu]] reálných čísel:
> - **Shora omezenou** existuje její supremum v $\mathbb{R}$.
> - **Zdola omezenou** existuje její infimum v $\mathbb{R}$.
> - **Shora i zdola omezenou** existuje jak její supremum, tak její infimum v $\mathbb{R}$.
> 
> *[[Číselné množiny#Reálná čísla|Co znamená to divné R?]]*

**Značení**
- Supremum množiny $M$ se značí jako $\sup M$.
- Infimum množiny $M$ se značí jako $\inf M$.

## Maximum a minimum
Pojmy **maximum** a **minimum** si asi každý dokáže představit. Jaký je ale rozdíl oproti [[#Supremum a infimum|supremu a infimu]]?

Rozdíl je v tom, jestli supremum a infimum **patří nebo nepatří do zkoumané množiny**.
- Pokud supremum ($\sup M$) **patří** do množiny, nazýváme ho **maximem množiny**.
- Pokud infimumum ($\inf M$) **patří** do množiny, nazýváme ho **minimum množiny**.

Z tohodle plyne, že maximum i minimum nemusí v množině existovat, ale **supremum a infimum** ano.