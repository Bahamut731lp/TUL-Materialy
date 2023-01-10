**Strom** je abstraktní datová struktura, která reprezentuje [[Vlastnosti grafu#Souvislost grafu|souvislý]] [[Vlastnosti grafu#Orientovanost grafu|neorientovaný]] [[Graf|graf]].

- Každý vrchol má $n$ potomků.
- Každý potomek má $1$ otce.

>[!tip] Vlastnosti stromu
>- **N-arita** - Kolik potomků může mít každý vrchol
>- **Hloubka** - Kolik potomků má vrchol "pod sebou"
>- **Šířka** - Kolik potomků je na dané hiearchické úrovni
>- **Pravidelnost** - Zda mají vrcholy stejný počet potomků
>- **Vyváženost** - Zda-li je strom automaticky vyvážený

>[!info] Běžné operace se stromy
>- **Hledání**
>- **Přidání vrcholu**
>- **Odebrání vrcholu**
>- **Přidání podstromu** (Prořezávání - *Pruning*)
>- **Odebrání podstromu** (Roubování - *Grafting*)
>- **Hledání kořene**
>- **Dotazování vlastností** (Hloubka, šířka, ...)
>- **Procházení stromu**

## Procházení (binárního) stromu
Stromy lze procházet **do šířky** (po "patrech") nebo **do hloubky** (po podstromech). Při procházení do hloubky lze rozlišovat mezi tím, v jakém pořadí provede operaci na uzlu, a procházení levého a pravého podstromu.
- **Preorder** - Nejdříve se provede akce na uzlu, poté se procháze větve
- **Inorder** - Nejdříve se provede akce na uzlech levého podstromu, poté na kořenu, a až poté na pravém podstromu
- **Postorder** - Nejdříve se provede akce na uzlech levého podstromu, následně pravého, a až na konec u uzlu.

>[!quote] Pořadí prvků při různých režimech procházení
>![[Pasted image 20221018163915.png]]


## Binární strom
Binární strom je takový strom, jehož vrcholy mají maximálně 2 potomky.