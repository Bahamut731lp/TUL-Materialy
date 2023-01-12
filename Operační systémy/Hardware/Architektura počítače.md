Za počítač považujeme systém, který se řídí nějakým teoretickým modelem hardware a dodržuje předem danou architekturu.

Dnes nejrozšířenější architekturou, která nebyla pořádně překonána, je [[#Von Neumannova architektura]], potamžo [[#Harvardská architektura]]

## Von Neumannova architektura
**Von Neumannova architektura** je architektura počítače, ve které je počítač řízen programem v paměti.

>[!example] Schéma Von Neumannovy architektury
>![[Pasted image 20221031225843.png]]

Podle Von Neumannovy archiktetury se počítač skládá z
- **Paměti** pro uchovávání programu, zpracováných dat a mezivýsledků
- **Řadiče** pro řízení činnosti počítače
- **[[Aritmetické obvody|Aritmeticko logické jednotky]]** pro výpočty
- **Vstupní jednotky** pro vstup programu a dat
- **Výstupní jednotky** pro výstup výsledků zpracované programem.

## Harvardská architektura
Harvardská architektura je obdoba [[#Von Neumannova architektura|Von Neumannovy architektury]], ve které je navíc oddělena paměť programu od paměti dat.

> [!example] Schéma Harvardské architektury
> ![[Pasted image 20221031230834.png]]

K oddělení paměti programu došlo z důvodu, že ve sdílené paměti bylo snadé chybou programátora poškodit nejenom data, ale i program jako takový. 

Dnes se s Hardvardskou architekturou setkáme hlavně na jednočipových počítačích (mikrořadiče).
