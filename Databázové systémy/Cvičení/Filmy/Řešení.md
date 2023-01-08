>[!example] Najděte názvy filmů, které režíroval Steven Spielberg.
>```sql
SELECT nazev
FROM Film
WHERE reziser = 'Steven Spielberg';
>```

>[!example] Najděte všechny roky filmů, které mají hodnocení 4 nebo 5
> - Výsledky seřaďte vzestupně.
>```sql
SELECT DISTINCT rok
FROM Film JOIN Hodnoceni on Film.id_film = Hodnoceni.id_film
WHERE hodnoceni >= 4
ORDER BY rok;
>```

>[!example] Najděte názvy všech filmů, které nemají hodnocení.
>```sql
SELECT nazev
FROM Film
WHERE id_film NOT IN (
>    SELECT id_film
>    FROM Hodnoceni
);
>```

>[!example] Někteří hodnotitelé neposkytli datum svého hodnocení.
> - Najděte jména takových hodnotitelů.
>```sql
SELECT jmeno
FROM Reviewer
WHERE id_reviewer IN (
>    SELECT id_reviewer
>    FROM Hodnoceni
>    WHERE datum IS NULL
);
>```

>[!example] Napište dotaz, které vrátí data o hodnocení v čitelnějším formátu.
>-  Jméno hodnotitele, název filmu, hodnocení a datum hodnocení. 
>- Setřiďte data podle jména
>	- hodnotitele
>	- názvu filmu 
>	- a nakonec podle hodnocení.
>```sql
SELECT DISTINCT jmeno, nazev, hodnoceni, datum
FROM Hodnoceni 
JOIN Reviewer ON Hodnoceni.id_reviewer = Reviewer.id_reviewer
JOIN Film ON Hodnoceni.id_film = Film.id_film
ORDER BY jmeno, nazev, hodnoceni;
>```

>[!example] Najděte nejvyšší hodnocení filmu od reviewera
>- Pro všechny případy, kdy určit reviewer hodnotil stejný film dvakrát a dal mu podruhé vyšší hodnocení, vraťte jméno reviewera a název filmu.
>```sql
SELECT DISTINCT jmeno, nazev
FROM Hodnoceni 
JOIN Reviewer ON Hodnoceni.id_reviewer = Reviewer.id_reviewer
JOIN Film ON Hodnoceni.id_film = Film.id_film
JOIN (
>    SELECT H1.id_reviewer, H1.id_film
>    FROM Hodnoceni as H1 
> 	   JOIN Hodnoceni as H2 
> 	   ON H1.id_film = H2.id_film AND H1.id_reviewer = H2.id_reviewer
>    WHERE H1.hodnoceni > H2.hodnoceni
) as Q 
ON Hodnoceni.id_film = Q.id_film AND Hodnoceni.id_reviewer = Q.id_reviewer;
>```

>[!example] Pro každý film, který má nějaké hodnocení
>- Najděte nejvyšší dosažené hodnocení. 
>- Vypište název filmu a hodnocení
>- Setřiďte podle názvu filmu.
>```sql
SELECT nazev, max(hodnoceni)
FROM Hodnoceni
JOIN Film ON Hodnoceni.id_film = Film.id_film
GROUP BY nazev
ORDER BY nazev, max(hodnoceni);
>```

>[!example] Pro každý film nalezněte název filmu a rozsah hodnocení
>- Rozsah hodnocení je rozdíl mezi nejvyšším a nejnižším hodnocením.
>```sql
SELECT nazev, max(hodnoceni) - min(hodnoceni) as Rozsah
FROM Hodnoceni
JOIN Film on Film.id_film = Hodnoceni.id_film
GROUP BY nazev
ORDER BY Rozsah DESC, nazev;
>```

>[!example] Najděte rozdíl mezi průměrným hodnocením filmů
>-  Uvedených před rokem 1980 a průměrný hodnocení filmů uvedených od roku 1980.
>- Ujistěte se, že jste spočítali průměrný hodnocení nejdříve pro každý film a pak průměr těchto průměrů před rokem 1980 a po roce 1980.
>```sql
SELECT nazev, max(hodnoceni)
FROM Hodnoceni
JOIN Film ON Hodnoceni.id_film = Film.id_film
GROUP BY nazev
ORDER BY nazev, max(hodnoceni);
>```

>[!example] Najděte jména všech reviewerů, kteří přispíli třemi a více hodnoceními.
>- Pokuste se napsat dotaz bez použití `HAVING` nebo bez `Count`.
>```sql
SELECT jmeno
FROM (
>    SELECT id_reviewer, count(hodnoceni) as pocet
>    FROM Hodnoceni
>    GROUP BY id_reviewer
>    HAVING count(hodnoceni) >= 3
) Prispevatele JOIN Reviewer on Prispevatele.id_reviewer = Reviewer.id_reviewer
>```