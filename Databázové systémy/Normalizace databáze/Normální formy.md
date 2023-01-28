Normální formy jsou pravidla, podle kterých určujeme, zda je databáze normalizovaná nebo ne.
Pokud relace nesplňují normální formu, [[Dekompozice|dekomponují]] se na menší relace, které už pravidlo splňují.

>[!tldr]
>- **1NF**: 
>	- Co hodnota to jedna věc
>	- každý řádek musí mít stejný počet sloupců
>- **2NF**: Každý sloupec musí být (alespoň nepřímo) závislý na celém klíči
>- **3NF**: Každý sloupec musí být přímo závislý na celém klíči

>[!error] První normální forma
>Relace je v první normální formě, pokud:
>- Každý atribut obsahuje jenom atomické hodnoty
>- Relace neobsahuje vícehodnotové atributy
>- Všechny $n$-tice mají stejný počet atributů

>[!example] Příklad
>Uvažujme relaci $Studenti(RC, jmeno, prijmeni, adresa, oceneni)$.
>- Adresa může být složena z vícero informací (ulice, PSČ, číslo domu, město, ...)
>- Ocenění může být vícehodnotové
>
>Aby byla relace v **1NF**, lze jí upravit takto:
>- $Studenti(RC, jmeno, prijmeni, ulice, mesto, psc)$
>- $Oceneni(RC, oceneni)$

>[!warning] Druhá normální forma
>Relace je v druhé normální formě, pokud:
>- Je v **první normální formě**
>- Každý neklíčový atribut je [[Funkční závislost|funkčně závislý]] na celém [[Klíče|klíči]]
>- Pro druhou normální formu postačí i [[Tranzitivnost|tranzitivní]] závislost

>[!example] Příklad
>Uvažujme relaci $Prihlasky(RC, jmeno, prijmeni, univerzita, adresa\_univerzity)$.
>- Adresa univerzity není funkčně závislá na klíči $\{RC, univerzita\}$
>- Jméno a příjmení také nejsou funkčně závislé na klíči
>
>Aby byla relace v **2NF**, lze jí upravit takto:
>- $Prihlasky(RC, univerzita)$
>- $Lide(RC, jmeno, prijmeni)$
>- $Univerzity(univerzita, adresa\_univerzity)$

>[!success] Třetí normální forma
>Relace je v třetí normální formě, pokud:
>- Je v **druhé normální formě**
>- Každý neklíčový atribut je závislý pouze na [[Klíče|klíči]]
>- Nesmí existovat [[Tranzitivnost|tranzitivní]] závislosti

>[!example] Příklad
>Uvažujme relaci $Prihlasky(RC, jmeno, prijmeni, univerzita, adresa\_univerzity)$.
>- Adresa univerzity není funkčně závislá na klíči $\{RC, univerzita\}$
>- Jméno a příjmení také nejsou funkčně závislé na klíči
>
>Aby byla relace v **2NF**, lze jí upravit takto:
>- $Prihlasky(RC, univerzita)$
>- $Lide(RC, jmeno, prijmeni)$
>- $Univerzity(univerzita, adresa\_univerzity)$

>[!tip] Boyce-Coddova normální forma
>Relace je v Boyce-Coddově normální formě, pokud
>- Je v **třetí normální formě**
>- Pravidla **třetí normální formy** platí pro všechny kandidátní klíče