Důkazy slouží k ověření pravdivosti [[Výroky|výroků]]. Pravdivost se ověřuje pomocí [[Axióm|axiómů]], definic a již dříve dokázaných vět.

## Druhy důkazů
Důkaz pravdivosti výroku můžeme provést několika způsoby, vždy se ale jedná o logický proces, který spoléhá na dodržování logických zákonitostí (např. pravdivostních tabulek [[Logické funkce|logických funkcí]]).

### Přímý důkaz
Používá se k dokazování implikace tím, že se výrok rozloží na řetězec menších pravdivých implikací.
>[!example] Proces přímého důkazu
>$$\Large\begin{cases}
 p &\implies q &\large\text{Původní výrok}\\
 p_1&\implies p_2 &\large\text{První krok}\\
 p_2&\implies p_3 &\large\text{Druhý krok}\\
 p_3&\implies p_4 &\large\text{Třetí krok}\\
 ...\\
 p_n&\implies q &\large\text{Poslední krok}\\
\end{cases}$$

### Nepřímý důkaz
Používá se k dokazování implikace tím, že se dokáže, že platí negovaná implikace
>[!example] Proces nepřímého důkazu
>$$\Large\begin{cases}
 p &\implies q &\large\text{Tvrzení}\\
 \neg{q} &\implies \neg{p} &\large\text{Nepřímý důkaz} \\
\end{cases}$$

Asi by nebylo od věci připomenou, že $p\implies q$ a $\neg{q} \implies \neg{p}$ jsou ekvivalentní výroky.

### Důkaz sporem
Důkaz je postaven na předpokladu, že negace výroku je pravdivá. Vezmeme negovaný výrok a sestavíme řetězec pravdivých implikací, ze kterých zjistíme, že negovaný výrok neplatí (dojdeme ke sporu). Když negace neplatí, tak musí platit původní výrok.

### Důkaz matematickou indukcí
