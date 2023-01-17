**Data Defininition Language** je [[Množiny|množina]] [[SQL|SQL příkazů]], které slouží k definování, změně a mazání [[Databázový objekt|databázových objektů]].

Při vytvoření [[Databázový objekt|databázového objektu]] se stává aktuální uživatel jeho vlastníkem.
```sql
CREATE TABLE nazev -- Vytvoří tabulku "nazev"
ALTER TABLE nazev  -- Pozmění tabulku "nazev"
DROP TABLE nazev   -- Kompletně vymaže tabulku "nazev"
TRUNK TABLE nazev  -- Vymaže data tabulky "nazev"
RENAME TABLE nazev -- Přejmenuje tabulku nazev
```

>[!example] Vytvoření tabulky `TEACHERS`
>```sql
>CREATE TABLE Teachers  
>(  
>	id_teacher Integer NOT NULL,  
>	id_office Integer NOT NULL,  
>	email Nvarchar(30) NOT NULL UNIQUE,  
>	name Nvarchar(30) NOT NULL,  
>	surname Nvarchar(30) NOT NULL,  
>	title_before Nvarchar(10) NULL,  
>	title_after Nvarchar(10) NULL,  
>	dob Datetime NOT NULL,  
>	type Integer NOT NULL CHECK (type > 0 AND type < 6)  
>	PRIMARY KEY (id_teacher),  
>	CONSTRAINT fk_TeachOffice FOREIGN KEY (id_office) -- pojmenování IO  
>	REFERENCES Offices(id_office),  
>	CONSTRAINT uc_NameSurnameDob UNIQUE (name,surname,dob) --přes více sloupců  
>);
>```

## Integritní omezení sloupců

|Omezení|Vysvětlivka|
|--:|:--|
|`NOT NULL`|Žádná hodnota v daném sloupci nesmí být `NULL`|
|`UNIQUE`|Všechny hodnoty v sloupci musí být unikátní|
|`PRIMARY KEY`|Sloupec je primárním klíčem|
|`REFERENCES`|Sloupec je cizím klíčem, definuje referenční integritu vzhledem k jiné tabulce|
|`CHECK`|IO zadané logickým výrazem|
|`DEFAULT`|Slouží k určení implicitní hodnoty sloupce (`NULL` nebo hodnota)|