## Z9-I-1
>Aritmetická posloupnost je taková posloupnost čísel, v níž je rozdíl každého čísla od čísla je mu předcházejícího stále stejný; tomuto rozdílu se říká diference. (Např. 2, 8, 14, 20, 26, 32 je aritmetická posloupnost s diferencí 6.)
>
>Bobek a Lolek mělí každý svou aritmetickou posloupnost. Jak Bolkova, tak Lolkova posloupnost začínala číslem 2023 a končila číslem 3023. Tyto dvě posloupnosti měly  26 společných čísel. Poměr Bolkovy a Lolkovy diference byl $5:2$.
>
>Určete rozdíl Bolkovy a Lolkovy diference.

Označme si 
- Bolkovu aritmetickou posloupnost velkým písmenem $B$
- $n$-tý prvek Bolkovy posloupnosti jako $b_n$
- diferenci v Bolkově aritmetické posloupnosti jako $db$
- Lolkovu aritmetickou posloupnost velkým písmenem $L$
- $k$-tý prvek Lolkovy posloupnosti jako $l_k$
- a diferenci v Lolkově aritmetické posloupnosti jako $dl$

Ze zadání víme, že 
- $b_1$ a $l_1 = 2023$ 
- $b_n$ a $l_k = 3023$
- Ve 26 případech platí, že $b_n = l_k$
- $\large\frac{db}{dl} = \frac{5}{2} \implies db = \frac{5}{2}dl$

a hledáme $|db - dl|$ (Absolutní hodnota je použitá, protože nás nezajímá, jakým "směrem" jsou rozdílný, ale akorát "o kolik" jsou rozdílný).


$$\large
\begin{aligned}
b_{n+1} - b_{n} &= \frac{5}{2}dl \\
l_{k+1} - l_{k} &= dl \\
\\
3023-2023 &= \frac{db}{n} \\
3023-2023 &= \frac{dl}{k} \\
\\
3023-2023 &= \frac{5}{2}dl\cdot\frac{1}{n} \\
3023-2023 &= \frac{dl}{k} \\
\end{aligned}
$$

## Z9-I-2
>Jsou dány dva shodné rovnostranné trojúhelníky $ABC$a $BDE$ tak, že velikost úhlu $ABD$ je větší než $120\degree$ a menší než $180\degree$ a body $C, E$ leží ve stejné polorovině vymezené přímkou $AD$. Průsečík $CD$ a $AE$ je označen $F$.
>
>Určete velikost úhlu $AFD$.

Ze zadání víme, že:
- Trojúhelníky $ABC$ a $BDE$ jsou **rovnostranné** (Strany trojúhelníku jsou stejně dlouhé)
- Trojúhelníky $ABC$ a $BDE$ jsou **shodné** (Oba trojúhelníky mají stejně dlouhé strany)
- $120\degree < ABD < 180\degree$

**Úvaha:**
- Potřebujeme trojúhelník $ADC$ (což je to samý $ADE$)


## Z9-I-3
> Tři kouzelníci kouzlí s čísly, každý však umí jen jedno kouzlo.
> - První kouzelník umí od libovolného čísla odečíst jedna
> - Druhý kouzelník umí libovolné číslo vydělit dvěma
> - Třetí kouzelník umí libovolné číslo vynásobit třema
> 
> Kouzelníci se při čarování mohou libovolně střídat, každý však může svoje kouzlo během jednoho vystoupení použít nejvýše pětkrát a žádný mezivýsledek nesmí být větší než 10.  Při jednom vystoupení měli z dané pětice číslic $3, 8, 9, 2, 4$ vykouzlit pětici trojek, při jiném vystoupení měli z téže pětice číslic vykouzil pětici pětek.
> 
> Jak si mohli s problémem poradit? Najděte možná řešení, nebo vysvětlete, proč to možné není.

Kouzelníci budou reprezentováni třemi funkcemi, které nějakým způsobem manipulují s číslem:
$$\large
\begin{aligned}
f(x) &= x - 1 &&\text{První kouzelník}\\
g(x) &= \frac{x}{2} &&\text{Druhý kouzelník}\\
h(x) &= 3x &&\text{Třetí kouzelník}\\
\end{aligned}
$$

V zadání je uvedeno omezení, že žádný mezivýsledek nesmí být větší než 10. Reálně to znamená, že obor hodnot funkce je shora omezen a nesmí být větší než deset.
$$\large
\begin{aligned}
f(x) &= x-1 &&\implies x-1 \le 10 &&\implies x \le \cancel{11}^{10}\\
g(x) &= \frac{x}{2} &&\implies \frac{x}{2} \le 10 &&\implies x < \cancel{20}^{10}\\
h(x) &= 3x &&\implies 3x \le 10 &&\implies x \le 3+\frac{1}{3}\\
\end{aligned}
$$

Tímto krokem jsme našli definiční obor našich kouzelníků.

Omezení definičních oborů $x < 11$ a $x < 20$ jsou sice obecně platné, ale v rámci úlohy nedávají smysl. Přece jenom se nemůže stát, že vstupem do funkce bude třeba 15, když tyhle vstupy, které jsou mezivýsledky od kouzelníků, nesmí být větší než 10. Proto jsou v předchozím zápise škrtnutý a nahrazený číslem 10.

Druhý kouzelník také není bez svých omezení. Protože pracujeme s přirozenými čísly, musíme mu dát pouze sudá čísla. Kdybychom totiž dělili dvoujkou liché číslo, dostanem zbytek a nebo zlomek, ze kterého už se nemáme jak jednoduše vysekat.

První kouzelník bude primární asistencí pro ostatní kouzelníky, bude totiž provádět malé úpravy tak, aby vše splnilo podmínky zadání, a nebo měnit sudost či lichost tím, že se odečte 1 (protože se lichá čísla od sudých liší právě jedničkou).

Když to shrneme:
- Třetí kouzelník může pracovat jenom s čísly menšími nebo rovny 3
- Druhý kouzelník může používat jenom sudá čísla
- První kouzelník umí měnit lichost či sudost čísel odečtením jedničky.

Protože má každý čaroděj omezený počet použití za vystoupení (tj. 5), tak při jejich skládání preferujeme používat co největší posuny směrem k číslu 3, to znamená, že chceme hlavně používat čaroděje 2 a 3 (funkce $h(x)$ a $g(x)$).

(Symbol $\circ$ značí složení funkcí, takže $(h \circ f)(x)$ je to samý, jako $h(f(x))$, takže se vezme výsledek funkce $f$ a použije se jako vstup pro funkci $h$)

|Číslo|Složení čarodějů pro přeměnu na číslo 3|
|:--:|:--:|
|1|$h(x)$|
|2|$(h\circ{g})(x)$|
|3|$-$|
|4|$f(x)$|
|5|$(f\circ{f})(x)$|
|6|$g(x)$|
|7|$(g\circ{f})(x)$|
|8|$(f\circ{g})(x)$|
|9|$(f\circ{g}\circ{f})$|

Takže pro vystoupení, kde mají pětici čísel $(3, 8, 9, 2, 4)$ překouzlit na $(3, 3, 3, 3, 3)$ tak, aby každ udělal maximálně 5 kouzel za vystoupení:

$$
\begin{bmatrix}
   3 \\
   8 \\
   9 \\
   2 \\
   4
\end{bmatrix}

\implies

\begin{bmatrix}
   3 \\
   (f \circ g)(8) \\
   (f \circ g \circ f)(9) \\
   (h \circ g)(2) \\
   f(4)
\end{bmatrix}

\implies

\begin{bmatrix}
   3 \\
   3 \\
   3 \\
   3 \\
   3
\end{bmatrix}
$$

Splnili jsme podmínku maximálně 5 kouzel?
- Prvního kouzelníka $f$ jsme použili 4krát
- Druhého kouzelníka $g$ jsme použili 3krát
- Třetího kouzelníka jsme použili jednou.

Našli jsme tedy jedno z možných řešení. Řešení je ale víc, to už je ale trochu jiná matika. Tohle je rozhodně jedno z těch úspornějších.

**Šlo by tedy i v dalších vystoupení vyčarovat i samé pětky?** 
Krátká odpověď: **Ne.**
Dlouhá odpověď:

Pojďme se podívat na to, kdy jednotliví kouzelníci vykouzlí číslo 5.
$$\large
\begin{aligned}
f(x) &= 5 &&\implies x-1 = 5 &&\implies x = 6\\
g(x) &= 5 &&\implies \frac{x}{2} = 5 &&\implies x = 10\\
h(x) &= 5 &&\implies 3x = 5 &&\implies x = \frac{5}{3}\\
\end{aligned}
$$

A my potřebujeme, aby pro všechna čísla z pětice (3, 8, 9, 2, 4) existovalo takové složení kouzelníků, které vykouzlí číslo 5. Než abych odůvoďnoval každé číslo zvlášť, upřel bych pozornost na číslo 4. 
- Protože potřebuju z čísla 4 vykouzlit číslo 5, musím ho nějakým způsobem zvětšit.
- Jediný kouzelník, který umí zvětšit číslo, je třetí kouzelník (Kouzelník $g$)
- Když ale třetí kouzelník zvětší číslo 4, dostaneme číslo 12
- 12 nesplňuje podmínku, že mezivýsledky nesmí být větší než 10.
- Další možnosti, jak ze 4 vykouzlit 5, by vyčerpaly prvního čaroděje natolik, že by nebylo možné dokouzlit další čísla.

## Z9-I-4
> Najděte nejmenší kladná celá čísla $a$ a $b$, pro která platí
> $$7a^3 = 11b^5$$

Zcela očividně tato rovnice platí pro $a, b = 0$, ovšem 0 nepatří do kladných celých čísel $a, b \gt 0$. To by musela být nezáporná (protože do nich 0 patří).

Protože pracujeme s celými čísly, musíme se přesvědčit, že je výsledek vůbec možný.

$$
\begin{aligned}
7a^3 &= 11b^5 \\
\frac{a^3}{b^5} &= \frac{11}{7} \\
\end{aligned}
$$

Nyní je tedy potřeba najít $a^3$, které vyplivne $11$ a $b^5$, které vyplivne $7$, resp. najít taková kladná celá čísla $a^3$ a $b^5$, jejichž poměr je $\frac{11}{7}$.

## Z9-I-5
>Na snovém tržišti nabídla Sfinga cestovali za čtyři sny sedm iluzí, dva šlofíky a jednu noční můru. Jinému cestovateli tatáž Sfinga nabídla za sedm snů čtyři iluze, čtyři šlofíky a dvě noční můry. Sfinga měří všem cestovatelům vždy stejně.
>
>Kolik iluzí stál jeden sen?

$$\large
\begin{aligned}
4s &= 7i + 2š + n  &&/\cdot(-2) \\
7s &= 4i + 4š + 2n \\
\\
-8s &= -14i -4š - 2n  \\
7s &= 4i + 4š + 2n \\
\\
-s &= -10i && /\cdot(-1)\\
\Aboxed{s &= 10i}
\end{aligned}
\;\;\;\;\;
\begin{cases}
s && ... &\text{sny} \\
i && ... &\text{iluze} \\
š && ... &\text{šlofík} \\
n && ... &\text{noční můry}
\end{cases}

$$

## Z9-I-6
> Vrcholy čtverce $ABCD$ spojuje lomená čára $DEFGHB$. Menší úhly u vrcholů $E, F, G, H$ jsou pravé a úsečky $DE, EF, FG, GH, HB$ po řadě měří 6 cm, 4 cm, 4cm, 1cm, 2cm.
>
>Určete obsah čtverce $ABCD$

Podle obrázku lze vidět, že jsou úsečky lomené čáry na sebe kolmé, tudíž si problém trochu zjednodušíme. Úsečky $DE$, $FG$ a $HB$ spojíme do jedné (tudíž $DEFGHB$) tak, že všechny dílčí úsečky posuneme tak, aby tvořili jednu dlouhou čáru. To samé uděláme pro $EF$ a $GH$. 

Proč to můžeme udělat? Každá dílčí úsečka, která se spojuje do té větší, má stejný směr. Ve finále je nám jedno, kde ta úsečka je, ale jak je dlouhá a v jakém je úhlu vzhledem k ostatním.

Po sečtení tedy máme 
- úsečku $DEFG$, která je dlouhá 12 cm.
- a úsečku $EFGH$, kteár je dlouhá 5 cm.

Vzhledem k tomu, že jsou na sebe úsečky kolmé, tak to křičí o použití Pythagorovy věty.

$$\sqrt{12^2 + 5^5} = 13$$

Vzhledem k tomu, že tato lomenná čára spojuje dva body, můžeme tvrdit, že se jedná o lomennou úhlopříčku, kde $DEFG$ je vychýlení směrem doprava, a $EFGH$ je vychýlení směrem dolů. Se znalostí toho, že to je úhlopříčka, a dokonce se znalostí její délky, můžeme dopočítat obsah původního čtverce.

Tím, že je to čtverec, tak má všechny strany stejně dlouhé, tedy vzoreček pro vypočítání úhlopříčky pomocí stran je

$$
\begin{aligned}
	\sqrt{a^2 + a^2} &= 13 \\
	\sqrt{2a^2} &= 13 \\
	\sqrt{2}\cdot a &= 13 \\
	a &= \frac{13}{\sqrt{2}} \\
\end{aligned}
$$

Obsah čtverce se počítá pomocí vzorce $a^2$, tudíž když teďko umocnímě obě strany rovnice, dostaneme ze vztahu pro délku čtverce jeho obsah.

$$
\begin{aligned}
	a &= \frac{13}{\sqrt{2}} \\
	a^2 &= \frac{169}{2} \\
	\Aboxed{a^2 &= 84,5\;\text{cm}^2} \\
\end{aligned}
$$