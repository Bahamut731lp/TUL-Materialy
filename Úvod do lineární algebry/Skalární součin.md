Skalární součin je operace, která dvěma vektorům přiřazuje číslo.

>[!tldr]
>- V komplexních prostorech je skalární součin pěkně na pytel

Skalární součin není nic jiného, než speciální [[Zobrazení|zobrazení]], které dvou [[Vektor|vektorům]] z nějakého [[Vektorové prostory|vektorového prostoru]] přiřadí číslo z [[Algebraické těleso|tělesa]], nad kterým je vektorový prostor definován.
>$$\LARGE T: \left<u|v\right> = t \in T$$
*Je-li definován vektorový prostor $U$ nad tělesem $T$ a je definováno zobrazení, které každé dvojici vektorů přiřadí číslo z tělesa $T$ skalárním součinem na prostoru $U$.* 

## Vlastnosti skalárního součinu

Aby skalární součin existoval, musí platit následující podmínky:

> *Mějme vektory $\vec{v}, \vec{u}, \vec{w}$ z prostoru nad [[Algebraické těleso|tělesem]] $T$*  a číslo $\alpha$ z tělesa $T$.
> $$\LARGE
\begin{aligned}
\left<u|v \oplus w\right> &= \left<u|v\right> + \left<u|w\right> \\
\left<u|\alpha \otimes v\right> &= \alpha \cdot \left<u|v\right> \\
\left<u|v\right> &= \left<v|u\right> \\
\left<u|u\right> &\ge 0 \\
\left<u|u\right> &= 0 \iff u = 0 
\end{aligned}$$

1. Musí být distributivní vůči sčítání
2. Musí být asociativní
3. Musí být komutativní
4. Skalární součin dvou stejných vektorů musí být větší než nula
	1. Pokud není vektor nulovým vektorem. Pak je nula