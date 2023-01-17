**Pohled** je virtuální [[Relační datový model|relace]] (tabulka), která je přizpůsobená specifickým potřebám uživatele. Používá se přimárně pro skrývání části dat, pro lepší řízení práv a modulárnímu přístupu k databázi.

>[!example] Vytvoření pohledu
>```sql
>CREATE VIEW pohled 
>AS ( vnoreny_dotaz )
>```

>[!example] Smazání pohledu
>Při mazání pohledu **nedojde** ke smazání dat.
>```sql
>DROP VIEW pohled 
>```

- K pohledům se z hlediska [[SQL|dotazování]] přistupuje jako ke klasickým tabulkám.

 ## Modifikace dat v pohledu
- Protože jsou pohledy akorát virtuální relací, není vždy modifikace dat možná.
- Lze definovat [[Trigger]], který určí, jak mají [[Data Manipulation Language|modifikace]] probíhat
- Lze také modifikace omezit

>[!example] Vytvoření pohledu
>Možnost `WITH CHECK OPTION` zajistí, že bude vyhozena výjimka pokaždé, když [[Data Manipulation Language|modifikace]] pohledu nebude v pohledu viditelná.
>```sql
CREATE VIEW ITPrijati2 AS  
SELECT sId, uJmeno  
FROM Prihlasky  
WHERE obor = 'IT' AND rozhodnuti = 'A'‚  
WITH CHECK OPTION;
>```