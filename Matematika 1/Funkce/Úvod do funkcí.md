# Úvod do funkcí
Funkce jsou v matematice druh objektů, se kterými mám já osobně *love-hate relationship*. Funkce jsou velmi užitečným nástrojem a zajímavým tématem, ale spoustou lidí zbytečně komplikovaný. Já se tedy pokusím popisovat funkce pokud možno tím nejjednoduším způsobem, který bude možný.

## Co je vlastně funkce?
Funkci si můžeme představit jako stroj, do kterého když vložíme nějaký vstup, tak on nám vyplivne nějaký výstup. 

Toť vše. Takhle fungují funkce.

Samozřejmě jak to vevnitř ten vstup zpracovává už je ta složitější část, a naším úkolem je ve většině případů právě zkoumat tento postup a jeho chování v různých hodnotách. 

## Předpis funkce
Postup, který funkce uvnitř provádí, je nějaký matematický zápis, kterému říkáme **předpis funkce**. Ten nám říká, co se konkrétně vevnitř se vstupem stane - například:
- $f(x) = x$ říká, že když do funkce zadáme $x$, tak nám to vrátí $x$
- $f(x)=\frac{x}{2}$ říká, že když do funkce zadáme $x$, tak nám to vrátí jeho půlku ($\frac{x}{2}$)
- $f(x)=\frac{5^x+7}{x^4}$ říká, že když do funkce zadáme $x$, tak to... eh... vrátí cokoliv výjde z $\frac{5^x+7}{x^4}$

Předpis funkce můžeme zapsat dvěma způsoby, které jsou si nazvájem rovny:
- Pomocí vstupní hodnoty: $f(x)=x$
- Pomocí výstupní hodnoty: $y=x$

Podle toho, co je za výraz v předpisu funkce, se poté jednotlivé funkce pojmenovávají.

## Jednoznačnost funkce
Když jsem říkal, že nám funkce něco vyplivne, když do ní dámě nějaký vstup - je velmi důležité, aby pro **každý vstup existoval pouze jeden výstup**. 

Je to jako kdybyste si v automatu třikráť naťukali číslo 31, a poprvé vám vypadla sušenka, napodruhé džus a napotřetí nic.

V matematice tedy platí, že:
>Pro každé $f(x)$ musí existovat **právě jedno** $y$.

## Základní pojmy k funkcím
Tenhle text je z pohledu matiky trochu nepřesnej, hlavně co se terminologie týče. Hodím Vám se na konec tedy tabulku základních pojmů, kterou budu naskrz dokumenty rozšiřovat.

Pro kompletní přehled koukněte do [[Terminologie]].

|Pojem|Význam|
|:--:|:--:|
|Jméno funkce|Název, pod kterým se funkce používá. Nejčastěji písmena $f, g, h, ...$|
|Parametr funkce|Jedná se o vstupy, se kterými funkce pracuje. Nejčastěji písmenko $x$|
|Argument funkce|Konkrétní parametr, s kterým funkci "voláme"|
|Funkční hodnota|Hodnota, kterou nám funkce vrátí po zavolání|