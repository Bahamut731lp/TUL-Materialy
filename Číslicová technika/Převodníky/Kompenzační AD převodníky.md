Kompenzační AD převodníky slouží k převodu [[Signál#Analogový signál|analogového signálu]] na [[Signál#Číslicový signál|číslicový (digitální) signál]]. 

Využívají k tomu myšlenku, že pokud máme nějaké vstupní napětí, tak ho použijeme jako referenci. Následně budeme D/A převodníkem prohánět postupně se zvětšující digitální signály, dokud se výsledek nedostane dostatečně blízko právě ke vstupní referenci. Z tohoto důvodu se jim říká **kompenzační**, protože se snaží vykompenzovat (dopočítat) napětí, dokud není $\pm$ stejné, jako vstupní napětí, které chceme převést.

## Kompenzační čítací
**Kompenzační čítací AD převodník** používá vnitřního čítače, jehož výstup je přiváděn na [[DA Převodníky]]. 
- Převedený signál (tzv. zpětnovazební signál) je pak následně porovnán v komparátoru $\text{KOMP}$
- Pokud je zpětnovazební signál větší, než velikost vstupního napětí, na komparátoru bude logická 1
- Při logické 1 na komparátoru se sepne hradlo $\text{AND}$, které zastaví čítač
- Čítač po zastavení napíše výsledek do paměti.

Nevýhodou tohoto převodníku je, že čítač musí vždycky počítat od 0, tudíž je převod o něco pomalejší.

>**Schéma zapojení $n$-bitového kompenzačního čítacího AD převodníku**
>
>![[Pasted image 20221130115549.png]]

## Kompenzační sledovací
**Kompenzační sledovací AD převodník** pracuje obdobně jako [[#Kompenzační čítací]], ale má čítač, který umí čítat obousměrně. Směr čítání je pak řízen komparátorem, kdy:
- Pokud je zpětnovazební napětí **větší než** vstupní ($U_{DA} \gt U_{IN}$), tak se **čítá dozadu** ($U_{DA}$ bude zmenšováno)
- Pokud je zpětnovazební napětí **menší než** vstupní ($U_{DA} \lt U_{IN}$), tak se **čítá dopředu** ($U_{DA}$ bude zvětšováno)

Díky tomu, že čítač sleduje vstupní napětí, není potřeba čítat od nuly, jelikož si to čítač již sám zkoriguje, ať mu dáme jakoukoliv arbitrární hodnotu napětí.


## Kompenzační s postupnou aproximací
**Kompenzační AD převodníky s postupnou aproximací** používají metody [[Bisekce|půlení intervalu]] pro urychlení kompenzace napětí.

>*Poznámka: Aproximace = Odhad, Přiblížení, ...*

Na začátku se do *aproximačního registru* napíše logická 1 na nejvyšší řád, a ostatní se nechají na logické 0.

>**Proč?** Protože tím velice rychle vytvoříme číslo, které je v polovině rozsahu převodníku

Následně se opakují kroky:
- Převeď hodnotu aproximačního registru pomocí DA převodníku
- Porovnej zpětnovazební napětí se vstupním napětím v komparátoru $\text{KOMP}$
- Výsledek z komparátoru zapiš do aproximačního (posuvného) registru, který se posune o 1 bit vpravo.
- **Opakuj tyto kroky, dokud z aproximačního registru napravo nevystoupí 1**

Po první logické 1, která bude vysunuta z aproximačního registru, se překlopí [[Klopný obvod RS|klopný obvod RS]], který ukončí převod a data z aproximačního registru se přepíší do paměti.

Velkou výhodou tohoto převodníku je, že převod trvá pevný počet kroků.

>**Schéma $n$-bitového kompenzačního AD převodníku s postupnou aproximací**
>
>![[Pasted image 20221130120337.png]]
