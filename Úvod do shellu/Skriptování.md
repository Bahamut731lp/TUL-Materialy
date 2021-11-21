# Skriptování
Skript je textový soubor, ve kterém jsou příkazy, které chceme, aby se vykonávaly.

Skripty psané v bashi nebo jiném shellu mývají příponu `*.sh` (není povinností). 

Soubor začíná **hlavičkou** (v angl. shebang, hashbang nebo sha-bang), která udává absolutní cestu k [[Interpretovaný jazyk|interpretu]]. Nejčastěji to bude `#!/bin/bash`. Hlavična není povinná, ale v rukou debila by to nemuselo být úplně košér, protože nevíme, jaký interpret by si to vzal na paškál.

## Proměnné
Proměnné slouží k ukládání hodnot, abychom na jejich hodnotu mohli později odkazovat - nečekaně. 

Proměnné se v bashi deklarují pomocí názvu a hodnoty. 
- Názvy jsou [[Case sensitivity|case sensitive]]
- Mezi názvem, rovná se a hodnotou **nesmí být mezery**
- Pro přístup k proměnné se před její název přidává **dolar**
```bash
#!/bin/bash
promenna=hodnota;
echo $promenna; #Vypíše "hodnota"
```

## Parametry
Do skriptu lze poslat parametry. Parametry se píší za cestu ke skriptu a ve skriptu se k ním přistupuje jako k očísleným proměnným od 0 do 9.

```bash
$ ~ skript.sh "parametr 1"
```

```bash
#!/bin/bash
echo $0; #Vypíše "parametr 1"
```

Kdyby parametrů bylo více jak 10, lze použít `shift` k vyhození prvního parametru, tím by se "posunuli" a na posledním místě by byl nový. Lze to takhle zacyklit pomocí `while` cyklu, a projít tak všechny parametry, dokud tam nějaké jsou.