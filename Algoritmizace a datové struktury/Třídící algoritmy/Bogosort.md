Bogosort je **třídící [[Algoritmizace a datové struktury/Algoritmy a složitost/Algoritmus|algoritmus]]**, který ke setřízení dat spoléhá na opakování náhodného rozmístění prvků, dokud se netrefí do seřazené [[Permutace|permutace]].

>[!example] Pseudokód bogosortu
>```js
>function bogosort(array) {
>	while (!isOrdered(array)) {
>		shuffle(array);
>	}
>}
>```

>[!bug] Že se o tom vůbec učíme
>Tenhle algoritmus byl vymyšlenej jako vtip a reálně nikde není použitej, ani by to nikoho normálního nenapadlo použít.