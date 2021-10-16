# Operace s komplexními čísly
S komplexními čísly lze počítat jako s reálnými čísly - máme tedy definované operace jako **sčítání** a **násobení**, stejně tak i **odečítání** a **dělení**. 
- Je ale výhodné se zamyslet, který tvar na kterou operaci používat
- V některých tvarech jsou totiž operace výrazně jednoduší

Pro umocnění a odmocnění komplexního čísla se používá [[Moivreova Věta]]

---
## Operace v algebraickém tvaru
### Sčítání a odčítání
Při sčítání komplexních čísel se sečtou zvlášť reálné a imaginární složky, obdobně to funguje u odčítání.

>$$\begin{aligned}
>\bar{A} &= \color{red}{3} \color{lime}+ 4j \\
>\bar{B} &= \color{red}{1} \color{lime}- 2j \\
>\\
>
>\bar{A}+\bar{B} &= (\textcolor{red}{3} + >\textcolor{lime}{1}) + (\textcolor{red}{4} + \textcolor{lime}{(-2)})j \\
>&=4+2j \\
>\\
>
>\bar{A}-\bar{B} &= (\textcolor{red}{3} - \textcolor{lime}{1}) + (\textcolor{red}{4} - \textcolor{lime}{(-2)})j \\
>&=2+6j \\
>\end{aligned}$$

### Násobení
Při násobení v algebraickém tvaru se roznásobí dvojčleny komplexního čísla:
>$$\begin{aligned}
>\bar{A} \cdot \bar{B} &= (a_1+b_1j) \cdot (a_2+b_2j) \\ &= a_1\cdot a_2 + a_1 \cdot b_2j + b_1j \cdot a_2 + b_1j \cdot b_2j \\
>&=(a_1 \cdot a_2 - b_1 \cdot{b_2}) + j\cdot{(a_1\cdot{b_2}+a_2\cdot{b_1})}
>\end{aligned}$$

### Dělení
K dělení v [[Úvod a tvary komplexních čísel#Algebraický tvar|algebraickém tvaru]] se využívá rozšíření zlomku komplexně sdruženým číslem[^1]

Tento proces je společně s násobením v [[Úvod a tvary komplexních čísel#Algebraický tvar|algebraickém tvaru]] složitý a zdlouhavý, navíc se tam lehce vloudí aritmetická chyba. Mnohem výhodnější je tyto operace provádět v [[Úvod a tvary komplexních čísel#Exponenciální tvar|exponenciálním tvaru]]

---
## Operace v exponenciálním tvaru
### Násobení
Při násobení komplexních čísel v [[Úvod a tvary komplexních čísel#Exponenciální tvar|exponenciálním tvaru]] stačí vynásobit reálné části a sečíst úhly imaginární části.

>$$\begin{aligned}
>\bar{A}\cdot{\bar{B}} 
>&= (|A|\cdot{e^{j\cdot{\varphi_A}}}) \cdot (|B|\cdot{e^{j\cdot{\varphi_B}}}) \\
>&= (|A|\cdot{|B|})\cdot e^{j\cdot({\varphi_A+{\varphi_B}})}\end{aligned}$$

### Dělení
Při dělení se postupuje obdobně jako násobení s tím rozdílem, že:
- Reálné složky se dělí
- a úhly v exponentu se odečítají

>$$\begin{aligned}
>\frac{\bar{A}}{\bar{B}} 
>&= \frac{(|A|\cdot{e^{j\cdot{\varphi_A}}})} 	{(|B|\cdot{e^{j\cdot{\varphi_B}}})} \\
>&= \frac{|A|}{|B|}\cdot e^{j\cdot({\varphi_A-{\varphi_B}})}\end{aligned}$$


[^1]:Komplexně sdružené číslo je takové číslo, jehož imaginární hodnota je opačná, tj. má opačné znaménko.

