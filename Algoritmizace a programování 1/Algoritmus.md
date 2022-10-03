# Algoritmus
Postup k řešení nějakého problému.

> **TL,DR:**
> - Algoritmus říká, jak řešit problém
> - Algoritmus by měl být **jednoznačný**, **konečný**, **obecný**, **srozumitelný** a **korektní**
> - 

# Vlastnosti algoritmu
1. **Jednoznačnost**
2. **Konečnost**
3. **Obecnost** 
4. **Srozumitelnost**
5. **Korektnost** 

---
## Jednoznačnost
- Algoritmus je **deterministický**[^2], neboli _předem určený_. 
- Je tudíž zaručeno, že při zadání stejných vstupních hodnot vždy dostanu stejné výsledky.

## Konečnost
 - Algoritmus je **rezultativní**[^1]
 - Proběhne v konečném počtu kroků a vždy vede k nějakému výsledku.

## Obecnost
- Algoritmus je **hromadný**
- Řeší určitou sadu problémů, které se liší akorát vstupem.

> Například počítání aritmetického průměru by mělo být nad jakýmikoliv čísly, nejenom na konkrétních číslech.

## Srozumitelnost
- Algoritmus by měl být **srozumitelný i pro ostatní**

## Korektnost
 - Algoritmus by měl dát pro správná vstupní data správný výsledek.
 
---
# Kritéria dělení algoritmů
## Iterativní vs. Rekurzivní algoritmy
- **Iterativní algoritmy** opakují jistou část kódu pomocí [[Cykly|cyklů]], 
- **Rekurzivní algoritmy** využívají [[Rekurze|rekurzi]] k opakování [[Funkce|funkcí]], [[Procedury|procedur]] či [[Metody|metod]].
- Algoritmy lze převádět mezi těmito podobami tam a zpátky.

## Deterministické vs. Nedeterministické
- **Deterministické algoritmy** mají v každém kroku jenom jednu možnost, jak pokračovat dále (např. [[Konečný automat|konečné automaty]])
- **Nedeterministické algoritmy** mají v nějakém kroku více možností, jak pokračovat dále.

> **Zmatení:** *Jednoznačnost algoritmu vs. Nedeterministický algoritmus*
> 
> Ve vlastnostech algoritmu píšu, že algoritmy mají být deterministický, ale zde se jako kritérium uvádí algoritmy nedetermenistické. Co s tím?
> 
> Rozdíl je v tom, jakým způsobem je zde determinovast myšlena, ve vlastnostech jde hlavně o fakt, že se na stejných datech chová vždycky stejně, a vrátí tak vždycky stejný výsledek (nehrajou tam žádné vnější vlivy či náhoda).
> 
> V rámci kritérií bych to spíše pojmenoval "**přímočarost**" - Jedná se totiž o rozdíl v tom, zda větvění programu závisí na vstupních datech či nikoliv.

> **TL:DR**: Jde o to, jestli větvení programu nezávisí na datech.
> - Nezávisí větvení na datech $\implies$ deterministický
> - Závisí větvení na datech $\implies$ nedeterministický

## Architektura algoritmu
- **Sekvenční algoritmy** jsou takové, jejichž kroky jsou vykonávány sekvenčně za sebou (daný krok "blokuje" vykonání dalšího kroku)
- **Paralelní algoritmy** jsou takové, kde může nastat souběžné vykonávání instrukcí, např. pomocí vláken.
- **Distribuovaný algoritmus** je vícevrstvá architektura, která je určena pro běh na vícero strojích.


[^1]: Rezultativní - Slovo přejaté z anglického slova **resultative**, které je zase odvozeno od slova **result** - výsledek.
[^2]:Deterministický - významově to znamená *předem určený*, což tady akorát říká, že dopředu víme, jak algoritmus skončí a neměl by tak dělat věci náhodně.