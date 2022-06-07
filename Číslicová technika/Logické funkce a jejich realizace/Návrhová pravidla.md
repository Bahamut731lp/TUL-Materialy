# Návrhová pravidla
Záměrné omezení možností návrhu, aby bylo možné zanedbat detaily a pracovat na vyšší úrovni abstrakce.

>**TL,DR:**
>- Pravidla určující, za jakých předpokladů a pomocí čeho bude obvod navržen
>- Dovolují neřešit titěrné detaily a soustředit se pouze na návrh

Další zjednéodušení návrhu přichází v podobě 

## Hiearchický návrh
Obvod lze rozdělit na menší obvody, které mezi sebou mají různé závislosti a společně tvoří hiearchii.

## Modularita
Modularita je vlastnost, která zaštiťuje dobře nadefinovaná rozhraní a funkce jednotlivých obvodů. Zkrátka chceme, aby se např. hodiny dobře ovládali a dělaly přesně, co mají.

## Regularita
Je opakované využívání již hotových modulů. Tím se výrazně snižuje čas potřebný na návrh celého obvodu.