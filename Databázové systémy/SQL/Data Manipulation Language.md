**Data Manipulation Language** je [[Množiny|množina]] [[SQL|SQL příkazů]], které slouží k aktualizování dat z [[Databázový objekt|databázových objektů]].

```sql
-- Vloží do tabulky název n-tici v závorce za klíčovým slovem VALUES
INSERT INTO nazev 
VALUES (...) 

-- Změní všechny hodnoty v sloupci "sloupec" na "hodnota" podle výběrové podmínky
UPDATE nazev 
SET (sloupec = 'hodnota')
WHERE (...)

-- Smaže řádky tabulky podle výběrové podmínky
DELETE FROM nazev
WHERE (...)
```