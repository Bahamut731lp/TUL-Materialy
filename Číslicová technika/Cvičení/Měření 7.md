# Měření 7
```vhdl
library IEEE;
use IEEE.STD_LOGIC_1164.ALL;
-- typy unsigned a signed
use IEEE.NUMERIC_STD.ALL;


entity counter_generic is
	-- Generic nám umožňuje nastavit "parametry" obvodu
	-- V tomhle případě to je šířka čítače, která je defaultně 4
    generic (
        C_WIDTH : integer := 4
    );
    port (
        clk : in std_logic;
        rst : in std_logic;
        enable : in std_logic;
        up_not_down : in std_logic;
        Q : out std_logic_vector(C_WIDTH - 1 downto 0)
    );
end counter_generic;

architecture Behavioral of counter_generic is
	-- Unsigned : Můžou se provádět aritmetické operace
    signal counter_reg : unsigned(Q'range); 

begin

    cyclic_counter : process(clk)
	    variable inc : integer := 1;
    begin
        if rising_edge(clk) then
            if rst = '1' then
                counter_reg <= (others => '0');
            elsif enable = '1' then
                if up_not_down = '1' then
	                inc := 1;
	            else
		            inc := -1;
                end if;
	            
	            counter_reg <= counter_reg + inc;
            end if;
        end if;
    end process;

    Q <= std_logic_vector(counter_reg);

end Behavioral;
```

```vhdl
library IEEE;
use IEEE.STD_LOGIC_1164.ALL;
-- typy unsigned a signed

entity top is
    port (
        clk : in std_logic;
        rstn : in std_logic;
        btn1, btnr, btnu, btnd, btnc : in std_logic;
        SW : in std_logic_vector(15 downto 0);
        LED: out std_logic_vector(15 downto 0);
    );
end top;

architecture Behavioral of top is
	-- Unsigned : Můžou se provádět aritmetické operace
    signal enable : std_logic;
    signal enable2 : std_logic;
    signal rst : std_logic; 

begin

    enable_button_debounce : entity work.pulse
	    port map(
		    clk => clk,
		    btn => btnl,
		    pulse => enable
	    );
	    
	citac_jenda : entity work.counter_generic
		generic map (
			C_WIDTH => C_WIDTH
		)
		port map (
			clk => clk,
			rst => rst,
			enable => enable,
			up_not_down => SW(0),
			Q => LED(C_WIDTH - 1 downto 0)
		)
	
	enable_button_debounce2 : entity work.pulse
	    port map(
		    clk => clk,
		    btn => btnr,
		    pulse => enable2
	    );
	    
	citac_vlad : entity work.counter_generic
		generic map (
			C_WIDTH => C_WIDTH
		)
		port map (
			clk => clk,
			rst => rst,
			enable => enable2,
			up_not_down => SW(1),
			Q => LED(15 downto C_WIDTH - 1)
		)


end Behavioral;
```

```vhdl
library IEEE;
use IEEE.STD_LOGIC_1164.ALL;
-- typy unsigned a signed

entity top_DUT is
end top_DUT;

architecture Behavioral of top_DUT is
	constant C_WIDTH : integer := 4;
	constant CLK_P : time := 10 ns;
	
	-- Unsigned : Můžou se provádět aritmetické operace
    signal clk : std_logic := '0';
    signal rst : std_logic := '0';
    signal enable : std_logic := '0';
    signal up_not_down : std_logic := '1';
    signal Q : std_logic_vector(C_WIDTH - 1 downto 0);
    signal limit : unsigned(C_WIDTH - 1 downto 0) 

begin
	clk <= not clk after CLK_P/2;

	DUT : entity work.counter_generic
		generic map (
			C_WIDTH => C_WIDTH
		);
		port map(
			clk => clk,
			rst => rst,
			enable => enable,
			up_not_down => up_not_down,
			Q => Q
		);

	TB: process
	begin
		rs <= '1';
		wait for CLK_P;
		rst <= '0';
		wait for CLK_P;
		enable <= '1';
		wait for CLK_P;
		wait
	end process;
end Behavioral;
```