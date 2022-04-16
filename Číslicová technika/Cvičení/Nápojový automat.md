# Nápojový automat
> Automat obsahuje otvor pro vhození malé či velké mince a dvě tlačítka pro volbu sodovky, nebo limonády. Po vhozeni malé mince lze volit sodovku, po vhození velké mince limonádu.Navrhněte logický obvod, který po vhození mince by při správné volbě tlačítka zapnul elektromagnet pro naliti zvoleného nápoje. V případě chybné volby vrátí minci zpět. Automat nesmí šidit ani majitele ani zákazníky

**Logické vstupy**
- Indikace vhozené velké mince, malé mince, požadavek na nalití sodovky, limonády.

**Logické výstupy**
- Napětí na elektromagnetu pro nalití sodovky, nalití limonády, vrácení mince.



```vhdl
library ieee;
use ieee.std_logic_1164.all;
 
entity Automat is
    Port(
        velka: in std_logic;
        mala: in std_logic;
        limonada: in std_logic;
        sodovka: in std_logic;

        magnetSodovka: out std_logic;
        magnetLimonada: out std_logic;
        vraceniMale: out std_logic;
        vraceniVelke: out std_logic;
    );
end entity;
 
architecture AutomatI is Automat
begin

    magnetSodovka <= sodovka and mala;
    magnetLimonada <= limonada and velka;
    
    vraceniMale <= mala and not(sodovka);
    vraceniVelke <= velka and not(limonada);

end architecture;
```