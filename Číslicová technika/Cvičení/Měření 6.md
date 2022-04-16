# Měření 5
```vhdl
library IEEE;
use IEEE.STD_LOGIC_1164.ALL;

-- Uncomment the following library declaration if using
-- arithmetic functions with Signed or Unsigned values
--use IEEE.NUMERIC_STD.ALL;

-- Uncomment the following library declaration if instantiating
-- any Xilinx leaf cells in this code.
--library UNISIM;
--use UNISIM.VComponents.all;

entity RS is
    Port (
        reset, set  : in std_logic;
        qn, q : out std_logic
    );
end RS;

architecture Behavioral of RS is
    signal a, b : std_logic;
begin

    a <= reset nor b;
    b <= set nor a;
    
    q <= a;
    qn <= b;
    
end Behavioral;
```

```bash
library IEEE;
use IEEE.STD_LOGIC_1164.ALL;

-- Uncomment the following library declaration if using
-- arithmetic functions with Signed or Unsigned values
--use IEEE.NUMERIC_STD.ALL;

-- Uncomment the following library declaration if instantiating
-- any Xilinx leaf cells in this code.
--library UNISIM;
--use UNISIM.VComponents.all;

entity Dlatch is
    Port (
        D: in std_logic;
        q : out std_logic;
        clk : in std_logic;
        enable, reset: in std_logic
    );
end Dlatch;

architecture Behavioral of Dlatch is
    signal a, b, v, u : std_logic;
begin

	-- q <= D when clk = '1'
	D_latch : process(reset, clk, D)
	begin
		if reset = '1' then
			q <= 0;
		elsif clk = '1' then
			q <= D;
		end if;
	end process;

end Behavioral;
```

```vhdl
library IEEE;
use IEEE.STD_LOGIC_1164.ALL;

-- Uncomment the following library declaration if using
-- arithmetic functions with Signed or Unsigned values
--use IEEE.NUMERIC_STD.ALL;

-- Uncomment the following library declaration if instantiating
-- any Xilinx leaf cells in this code.
--library UNISIM;
--use UNISIM.VComponents.all;

entity DFlipFlop is
    Port (
        D: in std_logic;
        q : out std_logic;
        clk : in std_logic;
        enable, reset: in std_logic
    );
end DFlipFlop;

architecture Behavioral of DFlipFlop is
    signal reg: std_logic;
begin

	-- q <= D when clk = '1'
	D_FlipFlop : process(clk)
	begin
		if rising_edge(clk) then
			if reset = '1'  then
				reg <= '0';
			elsif enable = '1' then
				reg <= D;
			end if;
		end if;
	end process;

	q <= reg;

end Behavioral;
```

```vhdl
library IEEE;
use IEEE.STD_LOGIC_1164.ALL;

-- Uncomment the following library declaration if using
-- arithmetic functions with Signed or Unsigned values
--use IEEE.NUMERIC_STD.ALL;

-- Uncomment the following library declaration if instantiating
-- any Xilinx leaf cells in this code.
--library UNISIM;
--use UNISIM.VComponents.all;

entity top is
    Port (
        SW: in std_logic(15 downto 0);
        LED : out std_logic(15 downto 0);
        LED_R, LED G, LED_B : out std_logic;
        CPU_RESETN, : in std_logic;
        BTNC, BTNU, CLK, BTNR, BTND: in std_logic; 
    );
end top;

architecture Behavioral of DFlipFlop is
    signal PAR_REG: in std_logic(SW'range);
    signal SER_REG: in std_logic(SW'range);
begin

	-- q <= D when clk = '1'
	PIPO_REG : process(CLK)
	begin
		if rising_edge(CLK) then
			if CPU_RESETN = '0'  then
				PAR_REG <= (others => '0');
			else
				PAR_REG <= SW;
			end if;
		end if;
	end process;
	
-- q <= D when clk = '1'
	SISO_REG : process(CLK)
	begin
		if rising_edge(CLK) then
			if CPU_RESETN = '0'  then
				SER_REG <= (others => '0');
			else
				--& slouží jako concat polí
				SER_REG(14 downto 0) <= SW(0) & SER_REG(SER_REG'high downto 1);
			end if;
		end if;
	end process;

	LED <= PAR_REG;
	
end Behavioral;
```

Latch = Obvod reaguje na hladiny obvod
Flip Flop = Obvod reaguje na hrany