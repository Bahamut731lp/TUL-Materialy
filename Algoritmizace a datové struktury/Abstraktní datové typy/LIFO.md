**LIFO** (Last In, First Out), někdy též nazývaná jako **fronta**, je homogenní, lineární a dynamický [[Abstraktní datový typ|abstraktní datový typ]], který data ukládá v pořadí, ve kterém byla vložena, a čtení probíhá od nejstaršího po nejnovější, tudíž ==výstup je ve stejném pořadí jako vstup==

>[!tldr]
>- **LIFO** = fronta
>- Při čtení ponechává pořadí vložení 
>- Poskytuje přístup pouze k vrcholu
>- Nové prvky lze vkládat pouze na začátek
>- Operace `create`, `push`, `pop` a `is_empty`

Frontu lze implementovat pomocí [[Algoritmizace a datové struktury/Strukturované datové typy/Pole|pole]] či [[Seznam|spojitého seznamu]].