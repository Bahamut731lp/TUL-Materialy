**Algoritmus Boyer-Moore** je algoritmus pro prohledávání řetězců, který stojí na myšlence zrcadlového hledání.

Existují tři situace, ve kterých se v okamžiku neshody nachází vzor
>[!info] Vzor obsahuje hledané písmeno
>Pokusíme se posunout vzor tak, aby se poslední výskyt hledaného písmena dostal naproti výskytu ve vzoru
>
>![[Pasted image 20230109074331.png]]

>[!info] Vzor obsahuje hledané písmeno, ale posun není možný
>Posuneme vzor o jeden znak
>
>![[Pasted image 20230109074428.png]]

>[!info] Vzor neobsahuje hledané písmeno
>Posuneme tak, aby vzor začínal na dalším prohledávaném písměně. Toto ne nejlepší případ, protože se posuneme o celý vzor.
>
>![[Pasted image 20230109074504.png]]

## Preprocessing
- Stejně jako u [[Knuth-Morris-Pratt]] algoritmu, tak i zde se posuny určují předem.
- Mapa abecedy a indexu, na kterém se vyskytuje poslední výskyt znaku (nebo -1)