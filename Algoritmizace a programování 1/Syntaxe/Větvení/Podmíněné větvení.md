Podmíněné větvení programu je způsob, jak větvit (rozdělit běh) program na vícero částí podle nějaké vyhodnocené podmínky.

V javě jsou k tomu vyhrazena klíčová slova `if`, `else if` a `else`.

```java
//Blok kódu, který se provede, pokud byla podmínka pravdivá
if (podminka) {
	System.out.println("1");
	System.out.println("2");
	System.out.println("3");
}

//Vykonání instrukce, pokud byla podmínka pravdivá
if (podminka) System.out.println("1");

```


## Úplné podmíněné větvení (if-else)


```java
if (podminka) {
	//Blok, který se vykoná, když byla první podmínka pravdivá
}
else if (podminka) {
	//Blok, který se vykoná, když nebyla první podmínka pravdivá
	//ale druhá podmínka byla pravdivá
}
else {
	//Pokud ani jeden předchozí blok nebyl pravdivý, vykoná se blok else
}
```