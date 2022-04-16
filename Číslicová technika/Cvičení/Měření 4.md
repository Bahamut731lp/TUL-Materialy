# Měření 4

```vhdl

-- HIGH downto LOW
-- LOW to HIGH

Port(
	s0: in std_logic_vector(1 downto 0);
	s1: in std_logic_vector(0 to 1);
);

```


```vhdl
----------------------------------------------------------------------------------
-- Company: 
-- Engineer: 
-- 
-- Create Date: 21.03.2022 12:36:30
-- Design Name: 
-- Module Name: mux41 - Behavioral
-- Project Name: 
-- Target Devices: 
-- Tool Versions: 
-- Description: 
-- 
-- Dependencies: 
-- 
-- Revision:
-- Revision 0.01 - File Created
-- Additional Comments:
-- 
----------------------------------------------------------------------------------

library IEEE;
use IEEE.STD_LOGIC_1164.ALL;

-- Uncomment the following library declaration if using
-- arithmetic functions with Signed or Unsigned values
--use IEEE.NUMERIC_STD.ALL;

-- Uncomment the following library declaration if instantiating
-- any Xilinx leaf cells in this code.
--library UNISIM;
--use UNISIM.VComponents.all;

entity mux41 is
    Port (
        a, b, c, d : in std_logic;
        s: in std_logic_vector(1 downto 0);
        q: out std_logic
    );
end mux41;

architecture Behavioral of mux41 is

--    constant cc : std_logic_vector(s'range) := "00";
--    constant c2 : std_logic_vector(2*s'length - 1 downto 0) := "0000";
    
--    VHDL pole jsou inclusive na oba konce
--    signal a : std_logic_vector(7 downto 0);
--    signal b : std_logic_vector(7 downto 0);
--    signal c : std_logic_vector(15 downto 0);
    
begin
      
    -- a <= X"80"; -- 1000 0000, X je pro označení decimálního zápisu
    -- a <= ('1', others => '0'); -- Udělá to samý, jako nahoře.
    
    -- c <= '0' &  "10" & a(7 downto 2) & b; -- Musí to sedět do délky pole (v tomhle případě 16)
    
    -- Tohle je sice pěkný, ale dá ty multiplexory za sebou, tedy tam vzniká zpoždění jako prase.
--    q <= a when s = "00"
--         else b when s = "01"
--         else c when s = "10"
--         else d; 

--    Mnohem lepší.
      with s select q <=
        a when "00",
        b when "01",
        c when "10",
        d when others;

end Behavioral;

```

```vhdl
----------------------------------------------------------------------------------
-- Company: 
-- Engineer: 
-- 
-- Create Date: 21.03.2022 13:30:48
-- Design Name: 
-- Module Name: seg - Behavioral
-- Project Name: 
-- Target Devices: 
-- Tool Versions: 
-- Description: 
-- 
-- Dependencies: 
-- 
-- Revision:
-- Revision 0.01 - File Created
-- Additional Comments:
-- 
----------------------------------------------------------------------------------


library IEEE;
use IEEE.STD_LOGIC_1164.ALL;

-- Uncomment the following library declaration if using
-- arithmetic functions with Signed or Unsigned values
--use IEEE.NUMERIC_STD.ALL;

-- Uncomment the following library declaration if instantiating
-- any Xilinx leaf cells in this code.
--library UNISIM;
--use UNISIM.VComponents.all;

entity seg is
    Port (
        value: in std_logic_vector(3 downto 0);
        position: in std_logic_vector(2 downto 0);
        cathode:  out std_logic_vector(6 downto 0);
        anode: out std_logic_vector(7 downto 0)
    );
end seg;

architecture Behavioral of seg is

begin

    with position select anode <=
        "11111110" when "000",
        "11111101" when "001",
        "11111011" when "010",
        "11110111" when "011",
        "11101111" when "100",
        "11011111" when "101",
        "10111111" when "110",
        "01111111" when others;
        
    with value select cathode <=
        "1000000" when "0000",
        "1111001" when "0001",
        "0100100" when "0010",
        "0011011" when "0100",
        "0010010" when "0101",
        "0000010" when "0110",
        "1111000" when "0111",
        "0000000" when "1000",
        "0011000" when "1001",
        "0001000" when "1010",
        "0000011" when "1011",
        "1000110" when "1100",
        "0100001" when "1101",
        "0000110" when "1110",
        "0001110" when others;      
                
end Behavioral;
```