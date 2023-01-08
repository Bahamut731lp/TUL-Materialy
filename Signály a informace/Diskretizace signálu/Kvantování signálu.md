Kvantování signálu je proces, který hladiny signálu převede na konečný počet [[Co znamená diskrétní|diskrétních hodnot]]. Jinak řečeno, jedná se o diskretizace oboru hodnot signálu.

>[!example] Kvantování spojitého signálu
>
>![[Quantized.signal.svg.png]]

## Distribuce kvantizačních úrovní
Hladiny (úrovně), na které se signál diskretizuje ("zaokrouhluje") se nazývají **kvantizační hladiny** (nebo **kvantizační úrovně**).

**Lineární kvantování**
V lineární distribuci kvantovacích úrovní se signál kvantuje na hladiny, které jsou od sebe stejně daleko, např. pomocí zaokrouhlování.

Aby nedošlo ke znatelnému zkreslení, doporučuje se pro $n$-bitový [[AD Převodníky|převodník]] mít $2^n$ kvantizačních hladin. 


**Nelineární kvantování**
Nelineární kvantování se používá tam, kde je zapotřebí konkrétnějši popsat určitou sekci hladin signálu. Příkladem z praxe je např. [A-Law](https://en.wikipedia.org/wiki/A-law_algorithm) nebo [Mu-Law](https://en.wikipedia.org/wiki/%CE%9C-law_algorithm).

## Kvantizační šum
Stejně jako u [[Vzorkování signálu|vzorkování]] platí [[Vzorkování signálu#Vzorkovací teorém|vzorkovací teorém]], i u kvantování platí jistá pravidla, za kterých nedojde ke znatelnému zkreslení signálu. Kvantování není nic jiného, než zaokrouhlování na určité hladiny, tudíž pokuď těhto hladin bude málo, bude se muset více zaokrouhlovat.

Chyba kvantování (zaokrouhlení) se ve výsledném signálu projevuje jako **kvantizační šum**, který může zásadně ovlivnit kvalitu výstupního signálu.

>[!example] Kvantizační šum
>
>![[Pasted image 20221130154701.png]]