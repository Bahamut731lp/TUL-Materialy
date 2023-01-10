Halda je případ [[Strom|stromu]], která navíc splňuje jednu z **podmínek haldy**, neboli
- Hodnota pomotka je vždy menší než jeho rodiče (**max-heap**)
- Hodnota pomotka je vždy větší než jeho rodiče (**min-heap**)

Halda se chová jako prioritní [[LIFO|fronta]].

## Binární halda
Binární halda je [[Strom#Binární strom|binární strom]],  pro který platí, že
- Je buď vyvážený
- Nebo se poslední úroveň zaplňuje zleva doprava

>[!example] Binární halda
>![[Pasted image 20230109025658.png]]

Konstrukce binární haldy je jednoduchá. Na spodní úroveň haldy přidáme nový uzel a porovnáme ho s rodičem, pokud jsou ve správném vztahu, končíme, jinak ho s ním prohodíme a opět porovnáváme, dokud nejsou ve správném vztahu

Jinak řečeno, nová hodnota "probublá" stromem nahoru, dokud nebude ve správném vztahu