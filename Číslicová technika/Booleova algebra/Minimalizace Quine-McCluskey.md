# Minimalizace Quine-McCluskey
**Quine-McCluskey** je název metody pro minimalizaci [[Booleovský výraz|logických funkcí]].

## Postup minimalizace
0. Funkci si převedeme na [[Booleovský výraz#Formy zápisu výrazu|UNKF]].
1. Negované proměnné nahradíme za 0, přímé proměnné za 1.
2. Členy seřadíme podle indexů a desítkových ekvivalentů a zapíšeme do tabulky (Index = počet jedniček v termu)

|Index|ABC|D. e.|
|:--:|:--:|:--:|
|0|000|0|
|1|010|2|
||100|4|
|2|011|3|
||110|6|
|3|111|7|

3. V řádcích lišících se v indexu o jedna, hledáme dvojice členů lišících se v jedné proměnné. *(Tuto proměnnou nahradíme pomlčkou a zapíšeme do nové tabulky)*

|Index|ABC|D. e.|
|:--:|:--:|:--|
|0|0-0|0, 2|
||-00|0, 4|
|1|01-|2, 3|
||-10|2, 6|
||1-0|4, 6|
|2|-11|3,7|
||11-|6,7|

4. Znovu najdeme řádky lišící se o jednu proměnnou a postup opakujeme. Stejné řádky škrtáme.

|Index|ABC|D. e.|
|:--:|:--:|:--|
|0|--0|0, 2, 4, 6|
||--0|0, 4, 2, 6|
|1|-1-|2, 3, 6, 7|
||-1-|2, 6, 3, 7|

5. Z výsledné tabulky zapíšeme výslednou funkci

|Index|ABC|D. e.|
|:--:|:--:|:--|
|0|--0|0, 2, 4, 6|
|1|-1-|2, 3, 6, 7|

$\large F_{(ABC)}=\overline{C}+B$