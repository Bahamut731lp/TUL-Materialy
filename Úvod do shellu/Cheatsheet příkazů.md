# Úvod do Shellu

|Příkaz|Vysvětlení|Příklad|
|:--:|:--|:--:|
|`who`|Vypíše uživatele přihlášené na zařízení||
|`pwd`|Vypíše pracovní adresář|

## Práce s adresáři
|Příkaz|Vysvětlení|Příklad|
|:--:|:--|:--:|
|`cd`|Vypíše uživatele přihlášené na zařízení||
|`ls`|Vypíše pracovní adresář||
|`mkdir`|Vytvoří adresář|`mkdir <nazev>`|
|`rmdir`|Odstraní (prázdný) adresář|`rmdir <nazev>`|
|`rm -r`|Rekurzivně smaže adresář|`rm -r <nazev>`|

## Práce se soubory
|Příkaz|Vysvětlení|Příklad|
|:--:|:--|:--:|
|`cat`|Vypíše obsah souboru|`cat <soubor>`|
|`mv`|Přesouvá soubor/adresář|`mv <co> <kam>`|
|`cp`|Kopíruje soubor/adresář|`cp <co> <kam>`|
|`touch`|Používá se pro vytvoření souboru|`touch <nazev>`|
|`rm -r`|Rekurzivně smaže adresář|`rm -r <nazev>`|
|`ls -l`|Zobrazení práva souborů|`ls -l <nazev>`|
|`chmod`|Mění práva souboru|`chmod <prava> <soubor>`|
|`chgrp`|Změní skupinu, které soubor patří|`chgrp <skupina> <soubor>`|
|`chown`|Změní vlastníka souboru|`chown <vlastnik> <soubor>`|

`chmod <prava> <soubor>` změní práva souboru
	- Práva lze zapsat po skupinách
		- Např. u - user, g - group, o - others, a - all
		- Taky lze pomocí dekadických hodnot (752 - rwx r-x -w-)

## Vstupy a výstupy
|Stream|Číslo|Význam|
|:--:|:--:|:--|
|`stdin`||Standardní vstup|
|`stdout`|1|Standardní vstup|
|`stderrout`|2|Standardní chybový vstup|

Přesměrování výstupu probíhá pomocí operátoru `>`.
- Jeden znak přepisuje soubor
- Dva přidává nakonec

|Stream|Význam|
|:--:|:--|
|`/dev/random`|Soubor s náhodnými znaky|
|`/dev/zero`|Soubor plný nul|
|`/dev/full`|Soubor simulující plný disk|
|`/dev/null`|Soubor, který se chová jako černá díra|

- `2 > /dev/null` - přesměrování chybového výstupu do černé díry

## Roura
`příkaz1 | příkaz2` - standardní výstup `příkazu1` se stane standardním vstupem `příkazu2`

`echo` vytiskne vstup
`cat` vytiskne obsah souboru
`wc` (word count) spočítá slova
`head` vytiskne část souboru, v parametru jde říct kolik řádků (`head -5` vytiskne 5 řádků)
`tail` vytiskne část souboru od konce
`grep` vyfiltruje vstup podle zadaného regulárního výrazu
`tr` změní znaky vstupu