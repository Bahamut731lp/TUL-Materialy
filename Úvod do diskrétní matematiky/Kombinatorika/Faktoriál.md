Faktoriál čísla $n$ je součin všech přirozených čísel menších než $n$

> [!tldr] TL,DR:
>- Faktoriál čísla $n$ je součin přirozených čísel menších než $n$
>- Výsledek se dá odhadnout pomocí **stirlingova vzorce**
>- $0! = 1$

Faktoriál je tedy v matematickém zápise definován jako

>[!example] Zápis faktoriálu:
>$$\large n! = 1 \cdot 2 \cdot 3 \cdot ... \cdot (n-1) \cdot n$$
>$$\large n \in \mathbb{N}$$

>[!tip] Rozložení faktoriálu:
>$$\large n! = (n-1)! \cdot n$$

## Faktoriál nuly
Obecně platí pravidlo, že **faktoriál nuly je jedna**.
>[!example] Faktoriál nuly
>$$\large 0! = 1$$

>[!help] Proč tomu ale tak je?
> Jednoduché vysvětlení je pomocí praktického použití faktoriálů. Faktoriály se totiž používají pro výpočet [[Permutace|permutací]].
> 
> Nula věcí lze uspořádat pouze do jedné množiny - a to konkrétně do prázdné množiny. 

## Stirlingův vzorec
Faktoriál díky svému výpočtu hodně rychle nabývá na hodnotě, abychom nemuseli ručně a zdlouhavě provádět výpočet faktoriálu, dá se výsledek odhadnout pomocí **stirlingova vzorce**

>[!info] Stirlingův vzorec
>$$\large n!\approx \sqrt{2 \cdot \pi \cdot n} \cdot \left(\frac{n}{e}\right)^n $$

Čím vyšší faktoriál počítáme, tím menší je odchylka.

## Výpočet faktoriálů pomocí logaritmů

$$\log(n!) \approx \frac{1}{2}\log(2\pi{n}) + n\cdot\log(n) - n\log(e) $$

## Rozšíření na reálná čísla
**Gamma funkce**