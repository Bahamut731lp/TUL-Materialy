**FIFO** (First In, First Out), někdy též nazývaná **zásobník**, je homogenní, lineární a dynamický [[Abstraktní datový typ|abstraktní datový typ]], který data ukládá v pořadí, ve kterém byla vložena, ale ==čtení probíhá opačně, neboli od nejnovějšího vloženého po nejstaršího==

>[!tldr]
>- **FIFO** = zásobník
>- Při čtení obrací pořadí vložení
>- Poskytuje přístup pouze k vrcholu
>- Nové prvky lze vkládat pouze na vrchol
>- Operace `create`, `push`, `pop`, `top` a `is_empty`

Zásobník lze implementovat pomocí [[Algoritmizace a datové struktury/Strukturované datové typy/Pole|pole]] či [[Seznam|spojitého seznamu]] a proměnné `top`, která si uchovává index vrcholu.

Operace `push` 
- přidává prvkek do vnitřního pole
- posouvá ukazatel `top` nahoru
- v případě použití pole o pevné délce kontroluje, zda již nedošlo k jeho zaplnění.

Operace `pop` 
- odebírá prvky z vnitřního pole, 
- posouvá ukazatel `top` dolů
- kontroluje, jestli není zásobník prázdný