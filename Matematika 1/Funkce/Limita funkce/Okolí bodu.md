# Okolí bodu
Okolí bodu, nejčastěji značeno písmenem epsilon ($\epsilon$), je vymezená oblast kolem nějakého bodu, ve kterém zkoumáme chování [[Posloupnosti|posloupnosti]] nebo [[Úvod do funkcí|funkce]].

> **TL,DR:**
> - Okolí bodu $U(a, \epsilon)$ je interval všech bodů $\left(r-\epsilon, r+\epsilon\right)$
> - Redukované okolí $R(a, \epsilon)$ je stejné jako okolí bodu, ale bez daného bodu $\left(r-\epsilon, r\right) \cup \left(r+\epsilon\right)$

## Jak určujeme okolí bodu
Okolí nejčastěji určujeme pomocí "poloměru" od našeho bodu.  Pokud bychom měli třeba bod v čísle 5, tak bychom si mohli vybrat okolí 3 ($\epsilon = 2$), pak by to na číselné ose vypadalo nějak takhle:

![[Pasted image 20211024232302.png]]

Okolí je tedy [[Intervaly|otevřený interval]] od spodní hranice okolí až po jeho horní hranici.

>Formální zápis s příkladem z obrázku výše:
> $$\large\begin{aligned}
> U(a, \epsilon) &= (r-\epsilon, r+\epsilon) \\
> U(5, 2) &= (5 - 2, 5 + 2)
> \end{aligned}$$

## Redukované okolí
Když vynecháme samotný bod, se kterým pracujeme (modrý bod z obrázku), tak dostáváme **redukované okolí**.

>Formální zápis s příkladem z obrázku výše:
> $$\large\begin{aligned}
> R(a, \epsilon) &= (r-\epsilon, r) \cup (r, r+\epsilon) \\
> R(5, 2) &= (5 - 2, 5) \cup (5, 5 + 2)
> \end{aligned}$$