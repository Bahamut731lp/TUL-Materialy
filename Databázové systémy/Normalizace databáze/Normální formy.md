Normální formy jsou pravidla, podle kterých určujeme, zda je databáze normalizovaná nebo ne.

## Nenormalizovaná forma (UNF)
Schéma relace je v **nulté normální formě** právě tehdy, když na něj nebyla doposud aplikována žádná normální forma.

## Nultá normální forma (0NF)
Schéma relace je v **nulté normální formě** právě tehdy, když existuje alespoň jeden atribut, který obsahuje více než jednu hodnotu

## První normální forma (1NF)
Schéma relace je v **první normální formě** právě tehdy, když jsou všechny atributy **atomické**, neboli je již nelze rozložit na menší atributy.

## Druhá normální forma (2NF)
Schéma relace je v **druhé normální formě** právě tehdy, když je splněna 1NF, a každý neklíčový atribut je funkčně závislý na [[Kandidátní klíč|kandidátním klíči]].

Jinak řečeno, nesmí existovat podklíč, který není plně závislý na primárním klíči.

## Třetí normální forma (3NF)
Schéma relace je v **třetí normální formě** právě tehdy, když je splněna 3NF a tabulka neobsahuje [[Tranzitivnost|tranzitivní]] závislosti. Jinak řečeno, neexistuje atribut, který by byl závislý na jiném atributu, který není [[Kandidátní klíč|kandidátním klíčem]].

Způsob, jakým lze třetí normální formu uspokojit je dekompozice tabulky, díky čemuž dosáhneme odstranění nalezené tranzitivní závislosti.

##
relace R je v BCNF tehdy a jen tehdy, když každý determinant (levá strana) funkční závislosti v relaci R je zároveň [[Kandidátní klíč|kandidátním klíčem]] relace R.