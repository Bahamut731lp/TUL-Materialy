# Úvod do Shellu
- `who` vypíše uživatele na serveru
- `pwd` *(Print Working Directory)* vypíše právě pracovní adresář
- `ls` - výpis adresáře. Lze doplnit cestu
	- Cesta může být relativní - `../../..`
	- nebo absolutní (z rootu) - `/home/...`

## Práce s adresáři
- `cd` *(change directory)* změní pracovní adresář
- `mkdir <cesta>` vytvoří adresář s názvem `cesta`
- `rmdir <cesta>` smaže adresář s názvem `cesta` (Adresář musí být prázdný)
- `rm -r <cesta>` smaže rekurzivně adresář
- `cat` vypíše obsah souboru
- `mv <co> <kam>` přesouvá adresář/položku
	- Funguje i pro přejmenovávání - v podstatě přesuneme na novou lokaci
- `cp <co> <kam>` *(copy)* - kopíruje adresář

## Práce se soubory
- `touch <soubor>` - mění timestamp souboru `soubor`
- `mv, cp, rm` funguje stejně jako u adresářů
- `ls -l <soubor>` zobrazí práva
- `chmod <prava> <soubor>` změní práva souboru
	- Práva lze zapsat po skupinách
		- Např. u - user, g - group, o - others, a - all
		- Taky lze pomocí dekadických hodnot (752 - rwx r-x -w-)
- `chgrp <skupina> <soubor>` - Změní skupinu souboru
- `sudo chown <vlastnik> <soubor>` - Změní vlastníka

## Vstupy a výstupy
`stdin` - Standardní vstup
`stdout` (1) - Standardní výstup
`stderrout` (2) - Standardní chybový výstup

Přesměrování výstupu probíhá pomocí operátoru `>`.
- Jeden znak přepisuje soubor
- Dva přidává nakonec

`/dev/random` - soubor s random znaky
`/dev/zero` - soubor samých null
`/dev/full` - simuluje plný disk
`/dev/null` - "černá díra"

`2 > /dev/null` - přesměrování chybového výstupu do černé díry

## Roura
`příkaz1 | příkaz2` - standardní výstup `příkazu1` se stane standardním vstupem `příkazu2`

`echo` vytiskne vstup
`cat` vytiskne obsah souboru
`wc` (word count) spočítá slova
`head` vytiskne část souboru, v parametru jde říct kolik řádků (`head -5` vytiskne 5 řádků)
`tail` vytiskne část souboru od konce
`grep` vyfiltruje vstup podle zadaného regulárního výrazu
`tr` změní znaky vstupu