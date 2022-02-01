# Vlastnosti grafu
[[Graf]] se dá dále upravovat v rámci podle toho, jakým způsobem potřebujeme vyjadřovat vztahy mezi vrcholy. Potřebujeme například vytvářet smyčky? Určovat směr z vrcholu do vrcholu? 

Níže jsou tyto vlastnosti vypsané a jakým způsobem mění název grafu. Podotýkám, že tyto názvy, lze kombinovat... takže můžeme klidně skončit s orientovaným multipseudografem <sup>fun times eh?</sup>. 

|Vlastnost|Název grafu|
|-:|:--|
|Jsou hrany v **uspořádané** dvojici?|Orientovaný|
|**Má** graf **více** stejně orientovaných hran?|Multigraf|
|**Nemá** graf **více** stejně orientovaných hran?|Prostý|
|Mohou se v grafu vytvářet smyčky?|Pseudograf|
|Existuje pro každé jeho dva vrcholy [[Sled]]?|Souvislý|

## Orientovanost grafu
- Pokud jsou hrany **neuspořádané** dvojice vrcholů
	- Mezi dvojicí je vztah "obousměrný"
	- takový graf nazýváme **neorientovaný**.
- Pokud jsou hrany **uspořádané** dvojice vrcholů
	- Mezi dvojicí je určen vztah "pouze jedním směrem"
	- takový graf nazýváme **orientovaný**[^1].

## Prostost grafu
- Pokud graf **neobsahuje** duplicitní hrany
	- mezi dvěma vrcholy neexistuje více stejně orientovaných hran, ale právě nanejvýš jedna
	- takový graf nazýváme **prostým**
- Pokud graf **obsahuje** duplicitní hrany
	- mezi dvěma vrcholy existuje více stejně orientovaných hran
	- takový graf nazýváme **multigrafem**

## Pseudograf
- Pokud umožníme vytvářet hrany mezi 1 vrcholem ($\large[V_i, V_i]$)
	- vytváříme smyčku ve vrcholu
	- takový graf nazýváme **pseudograf**

## Souvislost grafu
- Pokud pro každé dva vrcholy grafu existuje [[Sled|sled]]
	- takový graf nazýváme **souvislý**