

## Počet vláken
Pro získání počtu vláken lze využít možnosti formátování [[Správa procesů#Process Status|příkazu Process Status]] (`ps`) s možnostmi `-e` pro vylistování všech procesů, a možností `-o` pro specifikování vlastního formátu výstupu (můžeme si zvolit sloupce, které nás zajímají).

Pro každej proces nás zajímá jeho počet vláken, do možnosti formátu `-o` tedy uvedeme sloupec `thcount` (*thread count*) nebo `nlwp` (*number of lightweight processes*).

Příkaz `ps` vrátí hlavičku a následně data pro procesy, a protože nás zajímají akorát čísla, odřízneme hlavičku pomocí příkazu `tail`. S možností `-n` říkáme, kolik řádků chceme, a s hodnotou `+2` říkáme, že chceme od druhého řádku včetně.

Jednotlivé počty threadů máme na jednotlivých řádcích, proto je nějak potřebujeme sečíst. K tomu použijeme příkaz `awk`, který slouží pro práci s textem.

Nejdříve sečteme všechy hodnoty do pomocné proměnné `num_threads`, kterou na konci (`END`) vypíšeme pomocí příkazu `print`.

Zde je finální skript:
```bash
ps -eo thcount | tail -n +2 | awk '{ num_threads += $1 } END { print num_threads }'
```