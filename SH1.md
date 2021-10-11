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