Třída Scanner slouží ke čtení [[Streams API|datových proudů]]. Nejčasteji se používá pro čtení [[Standardní vstup a výstup|standardního vstupu]] nebo dat ze souboru.

```java
import java.util.Scanner;

Scanner reader = new Scanner(System.in);
```

Při načítání můžeme specifikovat, co za typ dat chceme načíst:

|Typ|Metoda|
|:--:|:--:|
|Celé číslo|`nextInt()`|
|Reálné číslo|`nextDouble()`|
|Byte|`nextByte()`|
|Řádek jako String|`nextLine()`|
