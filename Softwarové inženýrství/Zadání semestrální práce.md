- První verze 2 týdny před koncem semestru
- Vytvořit informační systém pro banku
- Potřebuju klienty, účty, platby, převody, měny, ...
- Účet má 1 až $n$ měn, tzv. **více zůstatků**
- Mockovat platby, logovat/historie
- Není potřeba měnit stav konta na přijímacím účtu
- Nelze mít záporný zůstatek
- Nejdřív se bere primární měna, poté CZK, poté odmítnutí platby
- Kurz je živý (ČNB ftw)
- Evidovat jméno a příjmení, + asi email pro 2FA
- Sepsat požadavky na výkon/software/prostředí

>[!Warning] Není potřeba vytvářet UI pro vytváření uživatele
>- Ale je to *cool*

>[!bug] Test coverage 80%!

>[!info] Use Cases
> - Platba (in/out), stačí přičítat/odečítat
> - Dvoufázové přihlášení, po kterém uvidím výpis a zůstatek
> - UI - Musí být responzivní (a asi to bude chtít PWA)

Bude se kontrolovat:
- 3 moduly: Klient, účet a platba
- 