# FPGA
**FPGA** (Field Programming Gate Array, česky *hradlová pole*) jsou tvořeny maticí programovatelných bloků.

Každý blok se skládá z 
- **CLB bloku** (Configurable Logic Block)
- **Vstupně výstupní blokem** (IOB)
- a propojením s propojovací maticí

>**Blokové schéma FPGA obvodu**
>
>![[Pasted image 20220606193657.png]]

## CLB
CLB jsou tvořeny 
- vyhledávací tabulkou (LUT)
- sekvenčním obvodem
- a dodatečnou logikou.

>**Blokové schéma CLB **
>
>![[Pasted image 20220606193908.png]]

Vyhledávací tabulka (Look-Up Table, LUT) je hardwarová realizace [[Pravdivostní tabulka|pravdivostní tabulky]]. Sekvenční obvod jsou používány pro realizaci sekvenční logiky.