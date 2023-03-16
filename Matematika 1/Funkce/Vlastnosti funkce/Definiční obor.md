# Definiční obor funkce
Jak jistě víte z [[Úvod do funkcí|úvodu do funkcí]], tak funkce mají tři základní stavební bloky:
- Parametry funkce (Vstupy)
- Předpis funkce (Postup pro zpracování vstupů)
- Funkční hodnoty (Výstup)

V matematice ale občas narazíme na situaci, kdy něco nemůžeme spočítat. Zkuste si třeba dělit nulou - moc daleko asi nedojdete...

Předpis funkce není nic jiného, než nějaký výpočet, do kterého dosazujeme čísla. Tím nám hrozí situace, že dosadíme číslo, se kterým nejde funkce spočítat.

Abychom věděli, co za čísla můžeme do funkce dosadit, tak si vytváříme tazvaný **definiční obor funkce**. 
-	Jedná se o [[Množiny|množinu]] všech čísel, které můžeme dosadit jako [[Úvod do funkcí#Základní pojmy k funkcím|argument funkce]].
-	Definiční obor funkce $f$ značíme jako $D(f)$[^1]

>[!example]
>$f: y=x \rightarrow D(f)=\mathbb{R}$
>$g: y=\frac{1}{x} \rightarrow D(f)=\mathbb{R}\setminus\set{0}$

Pojďme si shrnout příklad výše - do funkce $f$ můžu dosadit cokoliv z [[Číselné množiny#Reálná čísla|množiny reálných čísel]], protože ať tam dám, co tam dám, vždycky mi tam něco výjde.

Trochu horší to je s funkcí $g$, kde se mi parametr přesunul do jmenovatele. Vzhledem k tomu, že nemůžeme dělit nulou, tak tam můžeme dosadit jakékoliv reálné číslo kromě nuly ($\mathbb{R}\setminus\set{0}$)

---
## Jak poznat definiční obor funkce?
To je mnohem složitější otázka, než se zdá. Je to hlavně o analýze předpisu a znalosti principů jednotlivých funkcí.
- Víme, že nemůžeme dělit nulou $\implies$ [[Lomenné funkce]] nemohou mít nulu v definičním oboru
- Víme, že pod odmocninou musí být kladné číslo nebo nula
- ...

## Přehled definičních oborů

### Mocniné funkce
| Funkce | Definiční obor |
|:--:|:--:|
|Lineární|$D(f)=\mathbb{R}$|
|Kvadratická|$D(f)=\mathbb{R}$|
|Exponenciální|$D(f)=\mathbb{R}$|
|Logaritmus|$D(f)=\left(0,\infty\right)$|

### Goniometrické funkce
| Funkce | Definiční obor |
|:--:|:--:|
|Sinus|$D(f)=\mathbb{R}$|
|Cosinus|$D(f)=\mathbb{R}$|
|Tangens|$D(f)=\mathbb{R}\setminus\set{\frac{\pi}{2} + K\pi}; K\in\mathbb{Z}$|
|Cotangens|$D(f)=\mathbb{R}\setminus\set{K\pi}; K\in\mathbb{Z}$|

---
Analogicky k množině přípustných parametrů (přípustných $x$) existuje množina všech možných funkčních hodnot (všech $y$), která se nazývá [[Obor hodnot]].

[^1]: Že to vypadá jako zápis funkce? Velmi dobrý postřech. Technicky vzato to funkce je. Parametrem je nějaká jiná funkce, a výsledkem je množina všech přípustných argumentů pro danou funkci.