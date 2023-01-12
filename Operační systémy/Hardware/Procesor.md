



## Architektura procesoru

- Počet bitů adresní sběrnice (maximální adresa, kterou může použít)
- Skládá se z ALU, pracovních registrů, dekodéru instrukcí, řadiče a sběrnic

>[!faq] Jak souvisí architektura procesoru s operačním systémem?


## Vykonávání instrukcí
1. Instruction Fetch
2. Decode
3. Read data
4. Execute
5. Writeback

https://docs.google.com/presentation/d/1b3zk9ZWOM6G0iDKzm4fpu3Onkw04Icp2/edit?usp=sharing&ouid=108521459456700732808&rtpof=true&sd=true


## Režimy procesoru
Procesor dělí svojí činnost do několika (standardně minimálně dvou) režimů, ve kterém mají programy různá privilegia. Toto rozdělení slouží primárně k ochraně důležitých částí paměti, do kterých by, ať už to úmyslně či chybou programátora, mohli programy přistupovat neoprávněně.

Nejzákladnější rozdělení je na 
- **chráněný režim** (user mode)
- a **nechráněný režim** (kernel mode)

>[!info] Nechráněný režim
> V nechráněný režim má program přístup k celé paměti a k celé instrukční sadě. Standardně se v tomto režimu spouští [[Přerušení#Obsluha přerušení|obsluha přerušení]], která jsou vyvolána [[Systémová volání|systémovým voláním]].

> [!info] Chráněný režim
> V chráněném režimu je instrukční sada omezená, přístup k paměti je také omezen a důležité registry jsou chráněny.


