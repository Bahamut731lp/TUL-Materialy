# Derivace
Derivace funkce udává změnu její [[Úvod do funkcí#Základní pojmy k funkcím|funkční hodnoty]] v poměru k argumentu.

>[!tldr]
>- Derivace je tečna ke křivce, která popisuje rychlost změny funkční hodnoty a argumentu
>- Derivace se počítají pomocí směrnice sečny, kde se vzdálenost mezi body na sečně limitně blíží k nule
>$$\Large\lim_{h\to 0} = \frac{f(a + h) - f(a)}{h} = \frac{\Delta{y}}{\Delta{x}}$$
>tady je vzoreček pro dva body, což je v podstatě to samý, ale jinak napsaný:
>$$\Large\lim_{b\to a} = \frac{f(b) - f(a)}{b-a} = \frac{\Delta{y}}{\Delta{x}}$$
>

Pokud máme nějakou křivku, na které si zvolíme bod, tak derivace není nic jiného, než určení [[Předpis funkce|předpisu]] [[Tečna|tečny]][^2], která se dotýká právě v tomhle bodě.

>[!example] Derivace funkce $f(x)=x^2$ v bodě $D$
>![[Pasted image 20211026230823.png]]

K zjištění předpisu tečny (modré čáry) potřebujeme nějak odhadnout úhel $\alpha$, nebo nějak jinak vyjádřit její naklonění či **směr**. 

Vzhledem k tomu, že to je lineární funkce - neboli nějaká přímka, tak její směr můžeme vyčíst ze [[Směrnicový tvar přímky|směrnicového tvaru přímky]] - od toho se tak taky jmenuje, ne? Na výpočet [[Směrnicový tvar přímky#Směrnice přímky|směrnice přímky]] ale potřebujeme pracovat s [[Goniometrické funkce|goniometrickými funkcemi]], to znamená, že potřebujeme trojúhelník. 

Musíme mít na přímce tedy alespoň 2 body, abychom vytvořili pravoúhlý trojúhelník a mohli používat goniometrické funkce - tedy místo tečny musíme počítat se sečnou.

Vybereme si tedy bod další bod na křivce, který není totožný s derivovaným bodem, a vytvořím [[Sečna|sečnu]].
>[!example] Sečna procházejícím body $(a, f(a))$ a $(b, f(b))$
>![[Pasted image 20211026231911.png]]

Jak budeme vzdálenost mezi těmito body zmenšovat, tak bude sečna blíž a blíž připomínat námi hledanou [[Tečna|tečnu]].

>[!example] Body $C_1$ a $C_2$, které se blíží k bodu $A$
>Směrnice sečen, na kterých body $C_1$ a $C_2$ leží (čárkované čáry) se víc a víc blíží k námi hledané <span style="color: red">tečně</span>.
>
>![[Pasted image 20211026233029.png]]

Problém ale je, že se ať si body přiblížíme jak chcem, tak pořád nemůžeme tyto body spojit do jednoho, jinak bychom [[Směrnicový tvar přímky#Směrnice přímky|směrnici]] nemohli vypočítat[^1]. Máme tedy nějaký nástroj, který by nám ten druhý bod přiblížil nekonečně blízko? No samozřejmě. [[Limita funkce|Limity]].

> Zápis, kde se nám $b$ limitně blíží k $a$
> $$\Large\lim_{b\to a} = \frac{f(b) - f(a)}{b-a} = \frac{\Delta{y}}{\Delta{x}}$$

Body k sobě limitně přiblížíme tak blízko, že budou v podstatě jeden.

Pokud bychom si vzdálenost mezi těmi dvěma body ležícími na sečně označili nějakým písmenkem (např. $h$), tak můžeme zkoumat [[Limita funkce|limitu]], když by se tahle vzdálenost $h$ blížila k nule.

>[!example] Zápis pomocí vzdálenosti $h$
> $$\Large\lim_{h\to 0} = \frac{f(a + h) - f(a)}{h} = \frac{\Delta{y}}{\Delta{x}}$$
>![[Pasted image 20211026235429.png]]

Těmto limitám se říká **derivace v bodě funkce** a značíme jí jako název funkce s apostrofem (např. $f'(x)$).
- Počet apostrofů u názvu funkce říká, kolikátá derivace to je.
- Místo apostrofu se tam může objevit číslo či proměnná, což nám říká tu samou informaci

## Vlastní a nevlastní derivace
Stejně jako limity mohou být derivace **vlastní** nebo **nevlastní**
- Vlastní derivace má hodnotu rovnou nějakému [[Číselné množiny#Reálná čísla|reálnému číslu]]
- Nevlastní derivace má hodnotu $\pm\infty$.



[^1]: Vzhledem k tomu, že výpočet směrnice je podíl dvou rozdílů v hodnotách, tak by nám tam vyšlo $\frac{0}{0}$, což je dělění nulou a tím pádem nedefinovaná operace.
[^2]: Není to úplně pravda, protože neurčujeme předpis přímky, nýbrž její směrnici, jak se dočtete dál.