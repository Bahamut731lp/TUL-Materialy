Rekurze je vnořené volání stejné funkce.

> [!warning] Podmínky rekurze
>- Algoritmus má **ukončovací podmínku**
>- V každém kroku rekurze proběhne ke **zjednodušení problému**
>- Test ukončovací podmínky proběhne **před dalším voláním funkce**


**Přímá rekurze** - Funkce volá sebe sama, zatímco **nepřímá rekurze** volá jinou funkci, která eventuálně zavolá opět původní funkci (na hloubce nezáleží).

> [!danger] Rekurzi není vhodné použít když:
> - Máme k dispozici iterativní algoritmus se stejnou složitostí
> - Se chová nestabilně
> - Počet volání roste rychleji než lineárně

> [!tip] Tabelace rekurze
> Neefektivitu rekurze lze vyřešit tabelací, který si bude mezivýsledky ukládat a na začátku volání číst, jestli už se někdy náhodou pro stejnou kombinaci vstupů nespočítal výsledek