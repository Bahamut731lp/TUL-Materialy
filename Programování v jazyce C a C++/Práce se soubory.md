Soubory se v jazyce C čtou i zapisujou po blocích z disku do paměti a naopak. 

## Režimy otevírání souborů
Režim otevírání souborů je složen z různých příznaků, které metodě `fopen()` řeknou, jak má se souborem nakládat

>![[file-1.png]]

Příklad:
```c
//Deklarace pointerů na soubory
FILE *textFile;
FILE *binFile;

//Otevření binárního souboru (písmenko b) v režimu přepisování a případného vytvoření pro update
binFile = fopen("binar", "wb+");
//Otevření textového souboru v režimu přepisování
textFile = fopen("textovy.txt", "w");
```