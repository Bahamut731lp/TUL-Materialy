**Kruhový Buffer** (angl. *Circular Buffer*) je speciální případ [[FIFO|zásobníku]], který je díky své složitosti operací používán jako vyrovnávací paměť.

>[!info] Princip kruhového bufferu
>Kruhový buffer tvoří jedno [[Algoritmizace a datové struktury/Strukturované datové typy/Pole|pole]] a dva [[Ukazatel|ukazatele]]
>- Jeden ukazuje na první obsazený prvek (`head`)
>- Druhý ukazuje na první volný prvek (`tail`)
>- Při přidání prvku se `tail` inkrementuje v kruhu
>- Při odebrání se inkrementuje `head` a původní prvek smaže

>[!example] Přidávání a odebírání prvků v kruhovém bufferu
>![[circularqueueblockingbothgif.gif]]

>[!example] Anatomie kruhového bufferu
>>![[circular-queue-anatomy 1.webp]]