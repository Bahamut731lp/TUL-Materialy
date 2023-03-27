Tento dokument se snaží shrnout postup, jakým lze vyšetřovat konvergenci řady.


## Ověření nutné podmínky konvergence řady.
Jako první by se měla ověřit [[Nutná podmínka konvergence]], která nám dá vodítko k tomu, zda má vůbec smysl řadu vyšetřovat.

>[!quote] [[Nutná podmínka|Nutná podmínka]] konvergence řady:
>Řada $\sum_{n=1}^{\infty}a_n$ může konvergovat jen a pouze, když je $\lim_{n\to\infty}a_n = 0$

Pokud limita výjde nula, můžeme pokračovat s vyšetřováním. Pokud výjde jinak, píšeme, že je řada divergentní a máme hotovo.

## Použití kritérií konvergence
Jestliže už víme, že řada může konvergovat, je na čase použít kritéria konvergence. Nejčastěji se asi používají [[Odmocninové kritérium#Limitní odmocninové kritérium|limitní odmocninové kritérium]] a [[Podílové kritérium#Limitní podílové kritérium|limitní podílové kritérium]]. Samozřejmě se hodí znát i další kritéria, jako je např. [[Integrální kritérium]] či [[Srovnávací kritérium]].

## Vyšetření oboru konvergence
Některé řady mohu být zadány s parametrem (např. $\sum_{n=1}^{\infty}\frac{x-2}{n}$). Poté je potřeba vyšetřit, s jakými hodnotami parametru daná řada konverguje.

Máme-li nějakou mocninnou řadu, např. výše zmíněnou $\sum_{n=1}^{\infty}\frac{x-2}{n}$, postupujeme následovně:
1) Vypočítáme **střed oboru konvergence**, neboli $x-2 = 0 \implies x = 2$.
2) Vypočítáme **poloměr konvergence**
	1) Buďto pomocí "převráceného odmocninového kritéria" $(\lim_{n\to\infty}\sqrt[n]{a_n})^{-1}$
	2) nebo pomocí "převráceného podílového kritéria" $\lim_{n\to\infty}\left|\frac{a_{n}}{a_{n+1}}\right|$
