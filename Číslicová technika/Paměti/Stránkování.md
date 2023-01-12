Stránkování je technika rozdělení
- [[Logická paměť|logické paměti]] na úseky o pevné délce (*stránky*)
- a [[Fyzická paměť|fyzické paměti]] na úseky o stejné délce (*stránkové rámce*)

Slouží k rozdělení paměti tak, aby se nepoužívaná data (úseky programu) přesouvala mimo hlavní paměť, a zbytek byl uložen někde jinde (aby se program nemusel překládat).

Proto, jaká stránka má být načtená, slouží **tabulka stránek**. Ta je uložena v hlavní paměti a obsahuje informace o tom, k jaké logické stránce patří jaká fyzická stránka.

>[!example] Stránkovací mechanismus
>
>![[Pasted image 20220606222502.png]]

Nevýhodou je, že při větším logickém prostoru může tabulka zabírat značnou část hlavní paměti