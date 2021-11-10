# Lineární zobrazení
Lineární[^1] zobrazení (angl. *linear mapping* či *linear transformation*) je [[Zobrazení|zobrazení]] mezi [[Vektorové prostory|vektorovými prostory]] nad stejným [[Algebraické těleso|tělesem]], které zachovává operace sčítání a násobení skálárem.

>**TL,DR:**

---
## Jak jsme se k tomu dostali
Vzhledem k tomu, že lineární algebra není o ničem jiném než o velkém zobecňování a abstrakci, nejdříve se tedy podíváme na něco s trochu užší definicí - [[Lineární funkce]].

Mějme dvě [[Lineární funkce|lineární funkce]] ve [[Směrnicový tvar přímky|směrnicovém tvaru]], například:

>$$f(x)=2x + 3$$
$$g(x)=8x + 5$$

Co s těmito funkcemi můžeme dělat? Tak kromě dosazování je můžeme například sečíst a vynásobit bez toho, aniž bychom z toho udělali jiný druh funkce[^2]. Začněme sčítáním:

>$$\begin{aligned}
h(x) &= f(x) + g(x) \\
h(x) &= (2x + 3) + (8x+5) \\
h(x) &= 10x + 8
\end{aligned}$$

z toho nám vypadne nová funkce s vlastním předpisem. Předpis téhle nové funkce je tvořen z předpisů dvou našich původních funkcí. Tahle vlastnost, která nám dovoluje sečíst dvě funkce, se nazývá **aditivita** *(od slova slova adice - sčítání*).

Pojďme se ještě rychle podívat na násobení číslem
>$$\begin{aligned}
h(x) &= \alpha \cdot f(x) \\
h(x) &= \alpha \cdot (2x + 3) \\
h(x) &= 2\alpha\cdot{x} + 3\alpha \\
\\
\alpha &= 5 \\
h(x) &= 10x+15 \\
\end{aligned}$$

opět nám vypadne předpis, který je lineární funkcí. Tahle vlastnost, která nám dovoluje vytvořit $\alpha$-násobek funkce, se nazývá **homogenita**.

**Aditivita** říká, že je jedno, jestli nejdříve sečteme čísla v argumentu a poté aplikujeme funkci nebo naopak, **homogenita** říká to samé, ale pro násobení. 

Proč si vůbec tyhle vlastnosti vysvětlovat? Je to kvůli tomu, že [[Úvod do funkcí|funkce]] je speciální případ [[Zobrazení|zobrazení]], kdy množina obrazů je libovolná číselná množina. 

Zobrazení je tedy taková "obecnější verze" funkce, a jestliže tyhle vlastnosti platí pro [[Úvod do funkcí|funkce]], měli by platit pro [[Zobrazení|zobrazení]].

A když jsme tyto vlastnosti definovali pro [[Lineární funkce|lineární funkci]], tak je můžeme zobecnit do [[#Lineární zobrazení|lineárního zobrazení]].

---
## Definice lineárního zobrazení
Mějme dva [[Vektorové prostory|vektorové prostory]]:
- vektorový prostor $U(N, \oplus, \otimes)$
- vektorý prostor $V(M, \oplus, \otimes)$
- a oba dva tyto prostory jsou nad stejným [[Algebraické těleso|tělesem]] $T$[^3]

a mějme zobrazení $L$ z prostoru $U$ do prostoru $V$ ($L:U\to{V}$), které
- je **aditivní**
- a také je **homogenní**

tak poté takovému zobrazení říkáme **lineární zobrazení**.

---
## Vlastnosti lineárního zobrazení
- **Definiční obor** lineárního zobrazení generuje podprostor ve vektorovém prostoru **vzorů**
- **Obor hodnot** lineárního zobrazení generuje podprostor ve vektorovém prostoru **obrazů**
- Dimenze **oboru hodnot** lineárního zobrazení je jeho **hodností**
- Obrazem **nulového vektoru** je opět **nulový vektor**
- Lineární zobrazení **je prosté**, pokud [[Jádro zobrazení|jádro lineárního zobrazení]] obsahuje pouze nulový vektor

[^1]:Proč se mu říká lineární? Kdybychom udělali zobrazení mezi prostorem [[Číselné množiny#Reálná čísla|reálných čísel]] a dalších [[Číselné množiny#Reálná čísla|reálných čísel]], tak nám jako graf funkce výjde přímka (lat. *linea*).
[^2]: Výsledkem sčítání funkcí a násobení funkcí číslem bude opět ten samý druh funkce. Kdybychom například dělili, tak nám výjde funkce lomenná.
[^3]:Proč musí být nad stejným tělesem? Abychom mohli vektory z obou prostorů násobit "stejným číslem" (stejným prvkem tělesa)
