**Přerušení** je metoda pro asynchronní obsluhu událostí. Procesor přeruší vykonávání instrukcí a vykoná obsluhu přerušení. Následně po jejím dokončení pokračuje v předchozí činnosti.

>[!info] Typy přerušení
>Přerušení dělíme podle jejich původu na:
>- **Vnější (hardwarové) přerušení**
>- **Vnitřní přerušení**
>- **Softwarové přerušení**

## Řadič přerušení
**Řadič přerušení** je obvod, který obsluhuje žádosti o [[#Vnější přerušení|vnější přerušení]]. Vyhodnocuje jejich priority a následně je předává procesu ke zpracování.

>[!example] Schématické zapojení řadiče přerušení
>![[Pasted image 20230110161735.png]]

## Tabulka přerušení


## Vnější přerušení
**Vnější přerušení** je žádost o přerušení, která přichází ze vstupně výstupních zařízení. Tyto požadavky jsou vyhodnocovány [[#Řadič přerušení|řadičem přerušení]].

>[!example]- Příklady vnějšího přerušení
>- Stisk klávesy, tlačítka či jiného spínače
>- Pohyb myši
>- Požadavky tiskárny
>- Pevný disk oznamující, že má připravená data
>- Hrozící výpadek napájení
>- ...

## Vnitřní přerušení
**Vnitřní přerušení** je takové přerušení, které je vyvoláno samotných procesorem. Používá se k signalizování problémů při zpracování instrukcí, které jsou následnou obsluhou přerušení patřičně zpracovány.

>[!example]- Příklady vnitřního přerušení
>- Pokus o dělení nulou
>- Porušení ochrany paměti
>- Nepřítomnost matematického korpocesoru
>- Výpadek stránky paměti
>- ...

## Softwarové přerušení
**Softwarové přerušení** je takové přerušení, které je vyvoláno programem pomocí strojové instrukce `int` či jejímu ekvivalentu. Toto přerušení se používá pro volání služeb operačního systému z běžícího procesu. 

## Obsluha přerušení
Obsluha přerušení je zodpovědná za to, aby po skončení obsluhy byl uveden procesor do stavu jako na jejím začátku. Výpočet přerušené úlohy nesmí být ovlivněn.

>[!info] Proces obsluhy přerušení
>1. Procesoru je signalizováno přerušení
>2. Zkontroluje se, zda je obsluha přerušení povolena
>3. Dokončí se právě prováděná instrukce
>4. Do zásobníku se umístí adresa následující instrukce
>5. Podle tabulky přerušení se vyvolá proces, který je zodpovědný za obsluhu přerušení

>[!info] Proces návratu z přerušení
>1. Obsluha přerušení je ukončena instrukcí návratu z podprogramu (`RET`, `IRET`).
>2. Ze zásobníku je vyzvednuta návratová adresa. 
>3. Přerušená úloha bude pokračovat dále.