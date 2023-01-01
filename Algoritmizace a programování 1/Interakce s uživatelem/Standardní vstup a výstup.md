Standardní vstup a výstup (často zkracování na `std io`) jsou standardní [[Streams API|datové proudy]], které se používají ke komunikaci s uživatelem.

>[!tldr]
> - Standardní vstup a výstup slouží ke komunikaci s uživatelem.
> - Standardní vstup se označuje jako `stdin`, a je do něj směrován vstup z klávesnice.
> - Standardní výstup se označuje jako `stdout` a směřuje do terminálu.
> - Existuje standardní chybový výstup `stderr`, který taky jde do terminálu.
> - Výstupní proudy lze přesměrovávat.

Jako standardní vstup/výstup se používá **konzole** *(terminál)* - je to takové to černé okno, do kterého můžeme psát příkazy.

|Proud|Název|Zdroj/Cíl|
|--:|:--:|:--|
|Standardní vstup|`stdin`|Klávesnice|
|Standardní výstup|`stdout`|Terminál|
|Standardní chybový výstup|`stderr`|Terminál|

K ovládání standardních proudů se v Javě používá [[Třída System]].

