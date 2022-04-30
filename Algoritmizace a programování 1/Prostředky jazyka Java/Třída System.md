# Třída System
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

## Načítání ze standardního vstupu

