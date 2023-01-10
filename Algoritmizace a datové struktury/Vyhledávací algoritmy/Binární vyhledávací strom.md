**Binární vyhledávací strom** je [[Strom#Binární strom|binární strom]], ve kterém platí, že
- levý podstrom je vždy menší než kořen
- pravý podstrom je vždy větší než kořen

>[!example] Binární vyhledávací strom
>![[Pasted image 20230109050802.png]]

Implementací se liší od běžných [[Strom#Binární strom|binárního stromu]] v metodách pro vkládání a mazání, navíc s přídavkem metody pro hledání.


>[!info] Vkládání
>Najde se nejdříve správný rodič podle relací a poté se prvek připojí jako nový uzel
>
>![[Pasted image 20230109051233.png]]

>[!info] Mazání
>Při mazání mohou nastat dvě situace
>1. Mazaný uzel nemá potomky, můžeme ho prostě smazat
>![[Pasted image 20230109051603.png]]
>2. Mazaný uzel má jednoho potomka, poté se tento potomek přesune na místo mazaného uzlu
>   ![[Pasted image 20230109051659.png]]
> 3. Mazaný uzel má dva potomky
> ![[Pasted image 20230109051855.png]] 