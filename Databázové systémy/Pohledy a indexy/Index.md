**Indexování** je mechanismus pro zvýšení výkonnosti databáze. Obsahuje klíč vytvořený z jednoho či více [[Relační datový model|atributů tabulky]] a ukazatel na místo, kde jsou uložena data pro danej klíče.

Když se má vyhledat nějaký záznam (řádek), neprohledává se sekvečně tabulka, ale prohledává se index, který vrátí konkrétní místo na disku.

>[!example] Vytvoření indexu
>```sql
>CREATE [UNIQUE] [NONCLUSTERED] INDEX nazev_indexu
>ON tabulka(atribut | seznam_atributu)
>```

>[!example] Smazání indexu
>```sql
>DROP INDEX nazev_indexu
>```

>[!example] Vynucení použití indexu
>```sql
>SELECT *
>FROM tabulka WITH INDEX (nazev_indexu)
>```

>[!faq] Jaké datové struktury používají indexy?
> Indexy používají [[AVL Stromy|vyvážené stromové struktury]], nebo [[Hashovací funkce|hashovací funkce]].

>[!fail] Nevýhody indexování
>Indexování vyžaduje
>- Další místo na disku
>- Režii při vytváření indexů
>- Údržbu - když se změní data, musí se změnit i index

- Při indexování je potřeba vybalancovat rychlost dotazů a cenu aktualizací indexů.
- Chybějící indexy a přeindexovanost mohou vést k horšímu výkonnu

## Jak indexovat

### Úroveň tabulky (databáze)
- Jestli má smysl indexovat je otázka, kterou je potřeba zodpovědět pro každou tabulku zvlášť.

|Čtení|Zápis|Vhodný index|
|:--:|:--:|:--|
|Málo|Málo|Otázka, zda má vůbec smysl...|
|Málo|Hodně|Málo indexů a nad méně atributy|
|Hodně|Málo|Indexy nad více atributy|
|Hodně|Hodně|Záleží...|

### Úroveň dotazu
- Vhodné vytvořit indexy pro atributy, které se často vyskytují v podmínkách a při spojování tabulek

### Úroveň atributu
- Většina [[Databázové systémy|databázových systémů]] vytváří automaticky index nad primárním klíčem
- V indexu je dobré mít jako první atributy používané v podmínkách, až poté atributy s co nejvíce hodnotami
- Nemá smysl indexovat atributy, které mají málo různých hodnot

## Typy indexů
|Typ|Vysvětlivka|
|--:|:--|
|Úzký|Definovaný pouze nad jedním atributem|
|Široký|Definovaný nad více atributy|
|Hustý|Odkazuje na konkrétní záznam|
|Řídký|Odkazuje na stránku, na které je záznam|
|Primární|Obsahuje primární klíč|
|Sekundární|Neobsahuje primární klíč|
|Jedinečný|Definovaný nad `UNIQUE` atributem|

**Klastrovaný index** (Clustered Index) je setřízen fyzicky na disku podle nějakého [[Relační datový model|atributu]].
- Při zápisu dat je potřeba znovu setřídit
- Pro tabulku může být definován jenom jeden

**Neklastrovaný index** (Unclustered Index) netřídí data tabulky, ale akorát vytváří ukazatele na umístění dat
- Pro jednu tabulku jich může být vytvořeno víc