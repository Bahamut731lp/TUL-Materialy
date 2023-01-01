Některé prostředky jazyka Java mohou být **lokalizovatelné**. Když jsou třídy lokalizovatelné, znamená to, že je lze přizpůsobit k nějakému danému jazyku - například, zda se má použít desetinná čárka, nebo desetinná tečka.

```java
Scanner reader = new Scanner(System.in);

//Příklady
reader.useLocale(Locale.US);
reader.useLocale(new Locale("cs", "CZ"));

System.out.format(Locale.US, <formát>, <argumenty>);
```