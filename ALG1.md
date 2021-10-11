# Algoritmizace a programování 1
- Materiály na [elearningu](elearning.tul)

## Pojmy
- **Programovací jazyk** - prostředek pro zápis algoritmů

Programovací jazyk má několik vlastnostní, podle kterých je můžeme dělit.

### Úroveň abstrakce
- **NIžší jazyk** - Blíže k mikroprocesoru a JAS[^1]
	- Assembler, C, C++, Rust
- **Vyšší jazyk** - Blíže k lidskému jazyku.
	- Python, Ruby, Java, C#

### Podle druhu překladu
- **Kompilovaný jazyk** - Před během programu se projde celý program, zkontroluje se a kompletně se přeloží do strojového kódu
- **Interpretovaný jazyk** - Instrukce programu se překládají postupně za běhu. Vyžaduje interpret.

## Prostředky jazyka
- Zdrojový kód - zápis programu (txt)

### Třídy
- Jazyk Java je objektový => základem jsou **třídy**
- Pro funkční program je tedy potřeba **alespoň jedna** třída
- Třídy se ukládají do stejnojmenných souborů na disku
- Třídy jsou členěny do **balíků**
- Třídy z jiného balíku je třeba importovat *(kdo by to kurva řekl)*
- Struktura balíků musí odpovídat struktuře adresářů

Každý program v Javě má **vstupní bod** - jedná se o "začátek" programu.

```java
public static void main (String[] args) {
	...
}
```

Vstupních bodů (metoda `main`) může být v programu klidně víc. To, která se spustí, záleží na tom, kterou zadáne při spouštění programu. `java TestClass` spustí main metodu ve třídě `TestClass` .

Další třídy se deklarují následujícím způsobem:
```java
package alg1.jk.primitiva;
import java.util.scanner;

public class jmenoTridy {
	...
}
```

[^1]: Jazyk symbolických adres (běžně známo jako Assembler)