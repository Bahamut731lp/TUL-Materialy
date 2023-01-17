Integritní omezení udávají vlastnosti pro hodnoty atributů a [[Klíče|klíčů]] [[Relační datový model|relace]].

Mezi tyto vlastnosti patří:
- Doména atributu
- Povinnost hodnoty atributu (Přípustnost `NULL` hodnoty)
- Jedinečnost hodnoty atributu

>[!info] Integritní omezení pro [[Klíče#Primární klíč|primární klíč]]
>Všechny hodnoty atributů musí být povinné (nesmí být `NULL`)

## Referenční integrita
Referenční integrita zahrnuje požadavky na vztah mezi [[Klíče#Cizí klíč|cizím klíčem]] v jedné relaci a [[Klíče#Primární klíč|primárním klíčem]] v druhé relaci.

>[!important] Referenční integrita cizího klíče
>Když relace obsahuje cizí lkíč, musí se jeho hodnota
>- rovnat primárnímu klíči některé $n$-tice (řádku tabulky).
>- nebo být `NULL`

Pokud má být primární klíč, který je zároveň cizím klíčem v jiné relaci, vymazán nebo změněn, lze nastavit různé strategie pro zajištění referenční integrity.

|Strategie|Popis|
|--:|:--|
|`NO ACTION`|Řádek nepůjde smazat, protože na něj existují odkazy|
|`CASCADE`|Při smazání řádku se smažou i řádky, které na nej odkazují|
|`SET NULL`|Při smazání řádku se na místě cizích klíčů napíše `NULL`|
|`SET DEFAULT`|Při smazání řádku se na místě cizího klíče napíše výchozí hodnota|
|`NO CHECK`|Bez kontroly|