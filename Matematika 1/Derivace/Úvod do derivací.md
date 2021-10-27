# Derivace
Derivace funkce udává změnu její [[Úvod do funkcí#Základní pojmy k funkcím|funkční hodnoty]] v poměru k argumentu.

>**TL,DR:**
>- Derivace je tečna ke křivce, která popisuje rychlost změny funkční hodnoty a argumentu
>- Derivace se počítají pomocí směrnice sečny, kde se vzdálenost mezi body na sečně limitně blíží k nule
>$$\Large\lim_{h\to 0} = \frac{f(a + h) - f(a)}{h} = \frac{\Delta{y}}{\Delta{x}}$$
>nebo bez proměnné udávající vzdálenost:
>$$\Large\lim_{b\to a} = \frac{f(b) - f(a)}{b-a} = \frac{\Delta{y}}{\Delta{x}}$$
>

Pokud máme nějakou křivku, na které si zvolíme bod, tak derivace není nic jiného, než určení [[Směrnicový tvar přímky|směrnice]] tečny, která protíná právě tenhle jeden bod.

>Modrá čára je **tečna** ke grafu funkce $f(x)=x^2$ 
>Obrázek níže je **derivací funkce v bodě D**
>![[Pasted image 20211026230823.png]]

K zjištění směrnice té tečny (modré čáry) nemáme ještě dostatečné znalosti, ale mohli bychom ji odhadnou pomocí směrnice sečny, která bude dostatečně blízko.

Proč zrovna použít směrnici sečny? 
- Abychom dostali úhel, pod kterou je ta modrá čára, potřebujeme znát úhel $\alpha$
- Ten by se dal vypočítat pomocí [[Matematika 1/Funkce/Druhy funkcí/Goniometrické funkce|goniometrických funkcí]].
- Pro práci s goniometrickými funkcemi ale potřebujeme dvě strany trojúhelníku
- Trojúhelník vytvoříme vybráním si dalšího bodu na křivce a následným propojením bodů do pravoúhlého trojúhelníku

Vybereme si tedy bod, který bude nějak daleko od průniku tečny s křivkou.
>Sečna procházejícím body $[a, f(a)]$ a $[b, f(b)]$
>![[Pasted image 20211026231911.png]]

Jak budeme vzdálenost mezi těmito body zmenšovat, tak bude sečna blíž a blíž vypadat jako naše hledaná sečna.

>- Body $C_1$ a $C_2$ jsou blíž a blíž bodu $A$
>- Směrnice sečen, na kterých body $C_1$ a $C_2$ leží (čárkované čáry) víc a víc připomínají námi hledanou <span style="color: red">tečnu</span>
>![[Pasted image 20211026233029.png]]

Problém ale je, že se ať si body přiblížíme jak chcem, tak pořád nemůžeme tyto body spojit, jinak bychom směrnici nemohli vypočítat[^1]. Máme tedy nějaký nástroj, který by nám ten druhý bod přiblížil nekonečně blízko? No samozřejmě. [[Úvod do limit|Limity]].

> Zápis, kde se nám $b$ limitně blíží k $a$
> $$\Large\lim_{b\to a} = \frac{f(b) - f(a)}{b-a} = \frac{\Delta{y}}{\Delta{x}}$$

Pokud bychom si vzdálenost mezi těmi dvěma body ležícími na sečně označili nějakým písmenkem (např. $h$), tak můžeme zkoumat [[Úvod do limit|limitu]], když by se tahle vzdálenost $h$ blížila k nule.

>Zápis pomocí vzdálenosti $h$
> $$\Large\lim_{h\to 0} = \frac{f(a + h) - f(a)}{h} = \frac{\Delta{y}}{\Delta{x}}$$
> Oba zápisy říkají to samé.

>Zápis pomocí vzdálenosti $h$ v grafu.
>![[Pasted image 20211026235429.png]]

Těmto limitám se říká **derivace v bodě funkce** a značíme jí jako název funkce s apostrofem (např. $f'(x)$).
- Počet apostrofů u názvu funkce říká, kolikátá derivace to je.
- Místo apostrofu se tam může objevit číslo či proměnná, což nám říká tu samou informaci

## Vlastní a nevlastní derivace
Stejně jako limity mohou být derivace **vlastní** nebo **nevlastní**
- Vlastní derivace má hodnotu rovnou nějakému [[Číselné množiny#Reálná čísla|reálnému číslu]]
- Nevlastní derivace má hodnotu $\pm\infty$.



[^1]: Vzhledem k tomu, že výpočet směrnice je podíl dvou rozdílů v hodnotách, tak by nám tam vyšlo $\frac{0}{0}$, což je dělění nulou a tím pádem nedefinovaná operace.