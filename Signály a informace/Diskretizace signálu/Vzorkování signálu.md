**Vzorkování signálu** je proces, který ze [[Signál#Analogový signál|analogového signálu]] spojitého v čase udělá signál, který je v čase diskrétní (nespojitý). Jinak řečeno, jedná se o diskretizaci definičního oboru signálu

>[!example] Vzorkování
>
![[Vzorkování.png]]

## Vzorkovací teorém
**(Nyquistův) vzorkovací teorém** (neboli **podmínka vzorkování**) říká, že aby nedošlo ko ztrátě informace, musí být vzorkovací frekvence signálu **dvakrát vyšší než nejvyšší frekvence**.

>[!important] Nyquistova frekvence 
>$$\Large F_n = \frac{1}{2}f_s$$
>- $f_s$ je vzorkovací frekvence
>- $f_{max}$ je maximální frekvence
>
>Pak musí platit, že $F_n > f_{max} \equiv f_s > 2\cdot f_{max}$