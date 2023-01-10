Třída je struktura, která definuje, jaké budou mít [[Objekt|její instance]] **data** a **metody**.

>**TL,DR:**
>- Jsou to struktury předepisující **data** a **metody**
>- V Javě je na třídy vyhrazené klíčové slovo `class` s modifikátorem přístupu 

Pro definici tříd je vyhrazeno klíčové slovo `class`, které je zpravidla doplněno o [[Modifikátory přístupu|modifikátory přístupu]]. Každá [[Modifikátory přístupu#Veřejné konstrukce|veřejná]] třída v Javě je definována v odděleném souborech, jehož název se shoduje s názvem třídy. Třídy jsou pak dále děleny do [[Balíky|balíků]].

```java
//Tahle třída je uložena v souboru MojeTrida.java
public class MojeTrida {  
	// tělo třídy  
}
```

Každý [[Program|program]] musí mít **alespoň jednu třídu**, a alespoň jedna třída musí mít definovaný **vstupní bod programu** (to je, kde program začne vykonávat instrukce).

**Vstupní bod programu** je definován [[Metody|metodou]] `main` v následujícím tvaru:

```java
public static void main (String[] args) {  
	// tělo metody příkazy  
}
```
- `public` je [[Modifikátory přístupu|modifikátor přístupu]] označující, že je metoda [[Modifikátory přístupu#Veřejné konstrukce|veřejná]].
- `static` je klíčové slovo označující, že je pro všechny [[Objekt|instance třídy]] je metoda stejná.
- `void` je [[Datové typy a primitiva|datový typ]], který se používá v případě, že metoda nemá návratovou hodnotu
- `String[] args` je [[Algoritmizace a programování 1/Prostředky jazyka Java/Pole|pole]] vstupních argumentů, které mohou být uživatelem předány při spuštění programu.