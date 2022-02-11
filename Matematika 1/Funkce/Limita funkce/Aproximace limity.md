##  Aproximace limity
Pokud by přímé vyhodnocení limity nebylo možné, či by tomu bránily jiné okolnosti, lze ji v rozumné míře odhadnout. Odhadnout ji můžeme buďto z **grafu funkce**, nebo trochu přesněji z **tabulky funkčních hodnot** v [[Okolí bodu|okolí]] zkoumaného bodu.

### Pomocí grafu
Graf funkce je skvělým nástrojem, který nám pomáhá **odhadnout** konečnou funkční hodnotu v nekonečně malém okolí.

### Pomocí tabulky
Občas máme pod rukama složitou funkci, u které by bylo složité si jí představit či nakreslit graf. Pokud ale máme k dispozici kalkulačku, můžeme limitu aproximovat pomocí **tabulky**, ve které si vypočítáme hodnoty "nekonečně blízko" k limitnímu bodu a následně vytvoříme rozumný odhad.

> Příklad: Vypočtete následující limitu
> $$\large\lim_{x\to{3}}\frac{x^3-3x^2}{5x-15}$$

Tuto limitu budeme aproximovat pomocí tabulky, kdy si rozepíšeme bližší a bližší hodnoty z obou stran a limitu v nich vyhodnotíme.

|x|$\Large\frac{x^3-3x^2}{5x-15}$||x|$\Large\frac{x^3-3x^2}{5x-15}$|
|:--:|:--:|:--:|:--:|:--:|
|2,9|1,682||3,1|1,991|
|2,99|1,788||3,01|1,812|
|2,999|1,7988||3,001|1,801|

Z tabulky můžeme usoudit, že limita když se $x$ blíží 3 by mohla být 1,8.
$$\large\lim_{x\to{3}}\frac{x^3-3x^2}{5x-15} \approx 1,8$$