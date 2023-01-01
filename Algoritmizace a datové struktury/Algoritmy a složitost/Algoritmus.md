> [!INFO]
> Tenhle text navazuje na [[Algoritmizace a programování 1/Základy/Algoritmus]]

## Kritéria dělení algoritmů
### Iterativní vs. Rekurzivní algoritmy
- **Iterativní algoritmy** opakují jistou část kódu pomocí [[Cykly|cyklů]], 
- **Rekurzivní algoritmy** využívají [[Algoritmizace a programování 2/Rekurze|rekurzi]] k opakování [[Funkce|funkcí]], [[Procedury|procedur]] či [[Metody|metod]].
- Algoritmy lze převádět mezi těmito podobami tam a zpátky.

### Deterministické vs. Nedeterministické
- **Deterministické algoritmy** mají v každém kroku jenom jednu možnost, jak pokračovat dále (např. [[Konečný automat|konečné automaty]])
- **Nedeterministické algoritmy** mají v nějakém kroku více možností, jak pokračovat dále.

> [!help] Jednoznačnost algoritmu vs. Nedeterministický algoritmus
> Ve vlastnostech algoritmu píšu, že algoritmy mají být deterministický, ale zde se jako kritérium uvádí algoritmy nedetermenistické. Co s tím?
> 
> Rozdíl je v tom, jakým způsobem je zde determinovast myšlena, ve vlastnostech jde hlavně o fakt, že se na stejných datech chová vždycky stejně, a vrátí tak vždycky stejný výsledek (nehrajou tam žádné vnější vlivy či náhoda).
> 
> V rámci kritérií bych to spíše pojmenoval "**přímočarost**" - Jedná se totiž o rozdíl v tom, zda větvění programu závisí na vstupních datech či nikoliv.
> 
> **TL:DR**: Jde o to, jestli větvení programu nezávisí na datech.
> - Nezávisí větvení na datech $\implies$ deterministický
> - Závisí větvení na datech $\implies$ nedeterministický

## Architektura algoritmu
- **Sekvenční algoritmy** jsou takové, jejichž kroky jsou vykonávány sekvenčně za sebou (daný krok "blokuje" vykonání dalšího kroku)
- **Paralelní algoritmy** jsou takové, kde může nastat souběžné vykonávání instrukcí, např. pomocí vláken.
- **Distribuovaný algoritmus** je vícevrstvá architektura, která je určena pro běh na vícero strojích.