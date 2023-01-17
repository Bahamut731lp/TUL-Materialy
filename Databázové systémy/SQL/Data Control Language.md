**Data Control Language** definuje, jak k danému [[Databázový objekt|databázovému objektu]] mohou přistupovat další uživatelé.

>[!example] Přidávání práv
>- `WITH GRANT OPTION` umožní uživatelům, aby přidávali stejná či nižší práva dalším uživatelům
>- `PUBLIC` zajistí, že práva dostanou všichni nynější i budoucí uživatelé
>```sql
GRANT (seznam_privilegii | ALL PRIVILEGES)
ON nazev_db_objektu
TO (seznam_autorizacnich_identifikatoru | PUBLIC)
[WITH GRANT OPTION]
>```

>[!example] Odebrání práv
>- `GRANT OPTION` - Právo nebude odebráno, pokud mu bylo přiděleno ještě někým jiným
>- `CASCADE` - Odebrat práva všem, i těm, co je získali pomocí `WITH GRANT OPTION`
>- `RESTRICT` - Neumožní odebrat práva, pokud by `CASCADE` odebíral další práva
>```sql
>REVOKE [GRANT OPTION FOR] (seznam_privilegii | ALL PRIVILEGES)
>ON nazev_db_objektu
>FROM (seznam_autorizacnich_identifikatoru | PUBLIC)
>[RESTRICT | CASCADE]
>```