# Logické funkce
Logické funkce jsou, jak již název napovídá, [[Úvod do funkcí|funkce]], které pracují s logickými hodnotami - tj. **pravda** (1) a **nepravda** (0).

---
## Negace / NOT
Negace logické hodnoty je překlopení její aktuálni hodnoty do opačné, takže z pravdy bude nepravda a naopak.

|A|Negace A|
|:--:|:--:|
|0|1|
|1|0|

---
## Konjunkce / AND
Konjunkce logických hodnot, neboli **logický součin**, je funkce, která vrátí pravdu pouze tehdy, pokud jsou všechny její argumenty stejné

|A|B|A\*B|
|:--:|:--:|:--:|
|0|0|1|
|0|1|0|
|1|0|0|
|1|1|1|

---
## Disjunkce / OR
Disjunkce logických hodnot, neboli **logický součet**, je funkce, která vrátí pravdu tehdy, pokud alespoň jeden argument je pravda.

|A|B|A\+B|
|:--:|:--:|:--:|
|0|0|0|
|0|1|1|
|1|0|1|
|1|1|1|