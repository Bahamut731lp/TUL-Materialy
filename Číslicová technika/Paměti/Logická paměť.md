# Virtuální (logická) paměť
Systém několika pamětí, který je řízen tak, aby vytvářel paměťové prostory potřebné velikosti.
- Umožňuje vytvořit logické adresové prostory
- Každý prostor může být větší než je kapacita fyzického paměťového prostoru

Logické adresové prostory jsou realizovány ve vnější paměti (napří. na disku). Tento prostor se dá jednotně adresovat pomocí **logických adres**. Překlad těchto logických adres na fyzické zajištuje **jednotky pro správu paměti** (MMU - Memory Management Unit)

>**Blokové schéma zapojení mikroprocesoru a pamětí s MMU**
>
>![[Pasted image 20220606221323.png]]