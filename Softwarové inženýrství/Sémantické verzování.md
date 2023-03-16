**Sémantické verzování** je způsob číslování verzí softwaru, který odráží závažnost změn v nové verzi softwaru.

>[!info] Specifikace verzování
>- Sémantické verzování používá číslování ve tvaru `MAJOR.MINOR.PATCH-metadata`
>- V moment, co je číslo verze zavedeno, nesmí se měnit

- Číslo `PATCH` je zvyšuje jenom pokud došlo k opravě chyb. Tato změna musí být zpětně kompatibilní.
- Číslo `MINOR` se zvyšuje, pokud byla přidána funkcionalita, která zachovává zpětnou kompatibilitu.
- Číslo `MAJOR` se zvyšuje, pokud došlo k změnám, které způsobily zpětnou nekompatibilitu
- Při změne čísla se nulují čísla vpravo od něj
- Identifikátory v `metadata` se používá pro označení předběžných verzí.
- Identifikátory v `metadata` lze řetězit pomocí znaménka +

>[!example] Příklady verzování
>`2.1.0`,  `1.0.0-alpha`, `1.0.0-alpha.1`, `1.0.0-0.3.7`, `1.0.0-x.7.z.92`

>[!info] Definice sémantického verzování
>Sématické verzování je definování standardem na [této stránce](https://semver.org/lang/cs/).