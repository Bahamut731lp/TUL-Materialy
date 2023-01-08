# Komplexní čísla
Bohužel pro nás existují případy, kdy reálná čísla nestačí - resp. některé operace nejsou v reálných číslech definovány. Asi nejčastějším případem je například odmocnění záporného čísla.

Pro takovéhle případy vznikly čísla komplexní ($\mathbb{C}$-čísla), která se skládají ze dvou složek 
- **reálné složky** 
- a **imaginární složky**.

Komplexní čísla tedy vznikly tak, že se k ose **reálných čísel** přidala kolmá osa **čísel imaginárních**.
- Osa reálných čísel obsahuje všechna reálná čísla
- Osa imaginárních čísel obsahuje násobky imaginární jednotky $j$

>*Matematici běžně označují imaginární jednotku písmenkem **i**, já ji ale budu označovat písmenkem **j**, protože jsem si na to takhle zvykl v elektrotechnice, kde písmenko **i** je už zabrané pro proud - viz [[Praktické využití komplexních čísel]]*

---
## Důležité vztahy pro práci s komplexními čísly

Nejdůležitějším vzorcem v reálných číslech je tento:
>$$j^2 = -1$$

Tento vzoreček nám říká, že **imaginární část na druhou je rovna mínus jedničce**. 

Tuto definici lze rozšířit i pro další mocniny imaginární složky, kde platí následující tabulka: <sup>($n\in\mathbb{N}$.)</sup> 

|Odmocnina|Výsledek|
|:---:|:---:|
|$j^{4n}$|$1$|
|$j^{4n+1}$|$j$|
|$j^{4n+2}$|$-1$|
|$j^{4n+3}$|$-j$|


---
## Tvary komplexních čísel
Komplexní čísla lze reprezentovat v několika tvarech, mezi kterými lze převádět a ve kterých se některé operace provádí lépe než v jiných.

---
### Algebraický tvar
Nejzákladnějším tvarem je **algebraický tvar**, který nám říká velikosti jednotlivých složek. Píše se ve tvaru $a+b{j}$, kde $a$ je reálná složka a $bj$ je imaginární složka.

>[!example] Příklad komplexního čísla reprezentovaného na grafu
>$\bar{A}=3+4j$
>
>![[Pasted image 20211013231805.png]]

Pokud bychom chtěli zjistit vzdálenost od počátku souřadné soustavy, nebo-li "velikost" komplexního čísla, použijeme k tomu pythagorovu větu:

$$\large|A|=\sqrt{3^2+4^2}$$

Obecněji tedy zapsáno jako:
$$\large|A|=\sqrt{a^2+b^2}$$

---
### Goniometrický tvar
Goniometrický tvar nám uchovává informaci o
- vzdálenosti od počátku
- a úhlu naklonění

$$\large\bar{A}=(|A|\cdot\cos{\phi})+(|A|\cdot\sin{\phi})$$

> [!example] Příklad čísla prezentovaného v goniometrickém tvaru
>
>![[Pasted image 20211013232352.png]]

> [!info] 
> $$\begin{aligned} 
>A_{RE }&= |A| \cdot \cos{\varphi} \\
>A_{IM} &= |A| \cdot \sin{\varphi} \\ 
>|A| &= \sqrt{A_{RE}^2+A_{IM}^2} \\
>\varphi &= \arctan{ \frac{A_{RE}}{A_{IM} }}
>\end{aligned}$$

### Exponenciální tvar
Exponenciální tvar má hodně blízko ke tvaru goniometrickému, ale používá Eulerova čísla k vyjádření úhlu a imaginární složky.

$$\large\bar{A} = |A| \cdot e^{j \cdot \varphi}$$

---
Jak se s jednotlivými tvary pracuje a kdy je výhodné jaký použít se lze dočíst v dokumentu [[Operace s komplexními čísly]].