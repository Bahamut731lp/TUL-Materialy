Pro přístup ke [[Standardní vstup a výstup|standardním proudům]] lze použít Java třídu `System`, která má [[Atribut|atributy]] 
- `in` - pro ovládání standardního vstupu,
- `out` - pro ovládání standardního výstupu,
- `err` - pro ovládání standardního chybového výstupu.

Výpis na standardní výstup lze pomocí [[Metoda|metod]] `print` nebo `println`.  Metoda `print` vytiskne [[Argumenty programu|argument]] na standardní výstup, ale `println` ještě na konec přidá znak pro ukončení řádku.

```Java
System.out.print("ahoj");
System.out.print("ahoj");
System.out.print("ahoj");
//Vytiske:
//ahojahojahoj

System.out.println("ahoj");
System.out.println("ahoj");
System.out.println("ahoj");
//Vytiske:
//ahoj
//ahoj
//ahoj
```

## Formátování výstupu
Pro formátování výstupu lze použít metodu `printf` nebo `format` (jsou úplně stejné, akorát jiná jména).

Výstup se formátuje pomocí **specifikátorů formátu**, který každý začíná znamek `%` a každý reprezentuje jiný datový typ. Například `%s` je specifikátor datového typu `String`.

```Java
System.out.printf("Ahoj, %s!" ,"jméno");
//Vytiske:
//Ahoj, jméno!
```

## Načítání ze standardního vstupu

