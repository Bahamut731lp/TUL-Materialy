# Hazardy
Hazardy jsou krétké zákmity výstupní logické hodnoty do stavu opačného, než je předpokládaný stav. Hazardy jsou způsobeny nestejnou rychlostí signálu ve větvích obvodu, které se následně spojují dohromady.

>**Příklad obvodu s hazardem**
>Obvod má dvě větve: Jednu s invertorem, a jednu bez ní. Průchod signálu invertorem ho lehce zpozdí, čímž se větve "desynchronizují"
>
>![[Pasted image 20220606234309.png]]
>
>Časový diagram pak vypadá následovně:
>![[Pasted image 20220606234108.png]]

Hazardy v logických obvodech vznikají vlivem nedokonalostí a vlivem reálných vlastností základních prvků logických obvodů. Jiným důvodem pro vznik logického hazardu je samotný návrh a způsob realizace dané logické funkce, podle toho hazardy dělíme na
- **strukturální hazardy**, které vznikají vlastnostmi logických hradel a obvodů
- a **funkční hazardy**, které vznikají nevhodným návrhem a realizace logické funkce

Také rozlišujeme, kolikrát došlo k neočekávané změně hodnoty, podle toho se hazardy dělí na:
- **statické hazardy** (jedna neočekávaná změna hodnoty)
- **dynamické hazardy** (vícenásobná neočekávaná změna hodnoty)

>**Statický hazard**
>
>![[Pasted image 20220606235103.png]]

>**Dynamický hazard**
>
>![[Pasted image 20220606235206.png]]

*Pozn. **Statický hazard v logické 1** vzniká pouze v obvodu složeném ze **součinových logických hradel**, tedy AND, NAND, zatímco **statický hazard v logické 0** vznikne pouze v obvodu obsahujícím **součtová logická hradla**, tzn. OR a NOR.*