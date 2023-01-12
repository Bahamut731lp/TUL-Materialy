**Souběh** (angl. *race condition*) je situace, kdy dva procesy pracují nad stejnými daty, které bez jakéhokoliv řízení modifikují. 

V důsledku toho dochází k nekonzistenci dat, protože si mohou navzájem přepisovat výsledky.

>[!bug] Souběh je vždy chyba programátora.
>Pokud dojde k souběhu, vždy to je chyba programátora, který dostatečně neošetřil tzv. *kritické sekce* a *kritická data*.

>[!faq] Jak řešit souběh?
>Pro řešení souběhu je již spoustu metod, které jsou podporovány operačními systémy.
>Mezi ně patří například:
>- [[Atomické operace|Atomicita operací]]
>- [[Mutex|Zámky]]
>- [[Semafor|Semafor]]