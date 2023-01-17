**Trigger** je [[Procedury|procedura]] uložená na [[Databázové systémy|databázovém serveru]], která je automaticky spouštěna po nějaké události na základě spouštěcí podmínky.

>[!tldr]
> - Trigger je procedura, která se automaticky pouští po události v [[Databázové systémy|databázi]]
> - Používá se na komplexnější [[Integritní omezení|integritní omezení]] či přesunutí části logiky do prostoru databáze.
> - Syntaxe je hodně závislá na použitém [[Databázové systémy|DBMS]]

```SQL
CREATE TRIGGER jmeno
BEFORE | AFTER | INSTEAD OF udalost ON tabulka
[REFERENCING <referencni_promenne> AS <jmena>]
[FOR EACH ROW | FOR EACH STATEMENT]
WHEN (...)
[AS]
akce
```

## Spouštění triggeru
- `BEFORE` trigger pracuje s databází **před** provedení dotazu
	- Výhodné pro validace vstupních dat
	- Doplňování dat
- `AFTER` trigger pracuje s databází **po** provedení dotazu,
	- Výhodné pro aplikační logiku

## Granularita
- **Trigger na úrovni příkazu** (`FOR EACH STATEMENT`) je aktivován jednou pro celý příkaz
- **Trigger na úrovni řádku** (`FOR EACH ROW`) je aktivován pro každý modifikovaný řádek

>[!faq] Co když bude množina modifikovaných řádků prázdná?
>V tom případě se **trigger na úrovni příkazu** provede jednou, zatímco **trigger na úrovni řádku** se neprovede ani jednou. 
>
>*Makes sense.*

## Referenční proměnné
**Referenční proměnné** jsou takové proměnné, které odkazují na modifikované [[Databázový objekt|databázové objekty]] (řádky, tabulky, ...)

|Akce|Trigger na úrovni příkazu|Trigger na úrovni řádku|
|:--:|:--|:--|
|`INSERT`|`new_table`|`new_row, new_table`|
|`DELETE`|`old_table`|`old_row, old_table`|
|`UPDATE`|`new_table, old_table`|`new_row, new_table, old_row, old_table`|

>[!example] Příklad ON DELETE CASCADE referenční integrity pomocí triggeru na úrovni řádku
>```sql
>CREATE TRIGGER tr_cascade1
>AFTER DELETE ON Studenti
>REFERENCING old_row AS 0
>FOR EACH ROW
>	DELETE FROM Prihlasky WHERE Prihlasky.sID = 0.sID

>[!example] Příklad ON DELETE CASCADE referenční integrity pomocí triggeru na úrovni příkazu
>```sql
>CREATE TRIGGER tr_cascade2
>AFTER DELETE ON Studenti
>REFERENCING old_row AS 0
>FOR EACH STATEMENT
>	DELETE FROM Prihlasky WHERE Prihlasky.sID IN (SELECT sId FROM OT)
>```
