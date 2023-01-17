**Uložená procedura** je [[Procedury|podprogram]], který je uložený a spouštěný v rámci [[Databázové systémy|databázového serveru]].

>[!tldr]
>- Uložená procedura je blok kódu, který je uložen a vykonáván na [[Databázové systémy|databázového serveru]]
>- Používají se pro 
>	- validaci dat
>	- zapouzření často používaných příkazů
>	- Přesun programové logiky do DB

>[!example] Vytvoření procedury
>```sql
>CREATE [OR REPLACE] PROCEDURE jmeno
>[
>	(parametr1 [typ] datovy_typ),
>	(parametr2 [typ] datovy_typ),
>	...
>]
>[IS|AS deklarace_promennych]
>BEGIN
>	...
>	[EXCEPTION vyjimky]
>END;
>```

>[!example] Volání procedury
>```sql
>EXECUTE jmeno_procedury(parametr1, parametr2, ...);
>```

>[!example] Vymazání procedury
>```sql
>DROP PROCEDURE jmeno_procedury;
>```

>[!faq] Musí to být nutně [[Procedury|procedura]]?
>Samozřejmě, že ne. Může se také jednat o [[Funkce|funkci.]]