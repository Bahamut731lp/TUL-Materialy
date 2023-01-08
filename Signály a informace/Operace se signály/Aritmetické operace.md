## Posun
**Posun signálu** je operace, kterou můžeme prováděť na **definičním oboru** (neboli v čase) a i na oboru hodnot.

---
## Posun signálu v čase
Posun signálu v čase způsobí buďto

- **Zpoždění**, je-li posun záporný
- **Předstih**, je-li posun kladný

Pokud máme diskrétní signál $x[n]$, tak poté
- $y[n] = x[n-2]$ zpozdí signál o 2 vzorky.
- $y[n] = x[n+3]$ vytvoří předstih signálu o 3 vzorky.

> [!warning] Zpoždění posouvá signál "doprava", zatímco předstih ho posouvá "doleva"!

>[!example] Posun signálu v čase
>![[Pasted image 20221130162436.png]]

## Posun signálu v hodnotách
Posun signálu v hodnotách se způsobeno přičtením konstanty k hodnotě vzorku signálu.

>[!example] Posun signálu v hodnotách
>![[Pasted image 20221130164243.png]]
>
## Otočení
**Otočení signálu** je operace, kterou můžeme prováděť na **definičním oboru** (neboli v čase) a i na oboru hodnot.

---
## Otočení signálu v čase
Otočení signálu v čase způsobí "překlopení" podle vertikální osy

Pokud máme diskrétní signál $x[n]$, tak poté
- $y[n] = x[-n]$ otočí signál v čase

>**Otočení signálu v čase**
>
>![[Pasted image 20221130163823.png]]

## Otočení signálu v hodnotách
Otočení signálu v hodnotách způsobí "překlopení" signálu podle horizontální osy
Pokud máme diskrétní signál $x[n]$, tak poté
- $y[n] = -x[n]$ otočí signál v hodnotách

>**Otočení signálu v hodnotách**
>
>![[Pasted image 20221130163908.png]]
>
## Škálování
![[Pasted image 20221130164136.png]]

## Derivace

## Integrace