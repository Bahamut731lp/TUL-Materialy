# Matice sousednosti
Matice sousednosti je to taková matice, která popisuje, kolik hran vede z jednoho vrcholu do druhého.

Matice sousednosti je jedním ze způsobů reprezentace grafu. Tím, že se jedná o číselnou reprezentaci, je výhodná pro výpočty. 
- Matice je vždy čtvercová o velikosti $n\times n$, kde $n$ je počet vrcholů.

>$$\begin{bmatrix}
[V_1, V_1] & [V_1, V_2] & [V_1, V_3] & [V_1, V_4] \\
[V_2, V_1] & [V_2, V_2] & [V_2, V_3] & [V_2, V_4] \\
[V_3, V_1] & [V_3, V_2] & [V_3, V_3] & [V_3, V_4] \\
[V_4, V_1] & [V_4, V_2] & [V_4, V_3] & [V_4, V_4] \\
\end{bmatrix}$$
>Obecné schéma pro graf o 4 vrcholech, kde místo jednotlivých dvojic bude počet hran mezi body ve dvojici.

>|Obrázek grafu|Matice sousednosti grafu|
>|:--:|:--:|
>|![[Pasted image 20211108223746.png]]|$$\large\begin{bmatrix}0 & 1 & 0 & 0 & 0\\1 & 0 & 1 & 1 & 1\\0 & 1 & 0 & 1 & 0\\0 & 1 & 1 & 0 & 1\\0 & 1 & 0 & 1 & 0\end{bmatrix}$$|
>Příklad grafu a jeho matice sousednosti.