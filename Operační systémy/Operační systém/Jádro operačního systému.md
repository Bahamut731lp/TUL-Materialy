**Jádro operačního systému** je hlavní program operačního systému, který je při startu počítače zaveden do operační paměti a má plný přístup k systémovým zdrojům z nechráněného režimu.

## Typy jádra
K návrhu jádra lze přistupovat různými způsoby. Nejzákladnější dvě myšlenky byly, že buďto jádro [[#Monolitické jádro|dělá všechno]], nebo [[#Mikrojádro|nedělá skoro nic]]. V dnešní době se skončilo na jistém kompromisu mezi těmito myšlenkami.

### Monolitické jádro
**Monolitické jádro** je architektura jádra, kdy jsou všechny funkce operačního sysétmu implementovány do jednoho programu v nechráněném režimu. 

S jádrem procesy interagují skrz [[Systémová volání|systémová volání]], která jsou jádrem poskytována.

Nevýhodou monolitického jádra je neflexibilita, která přichází s jednotným celkem. V moment, co bychom chtěli něco změnit či přidat, museli bychom udělat novou verzi celého jádra.

>[!info] Moduly
>Moderní monolitická jádra mají tzv. **moduly**, které lze za běhu jádra přidávat a spouštět v nechráněném režimu. S tím ovšem přichází problém fragmentace paměti[^1] a bezpečnostní rizika.

>[!example] Schéma monolitického jádra
>![[Pasted image 20230112022754.png]]

### Mikrojádro
**Mikrojádro** je architektura jádra, která se snaží všechnu funkcionalitu rozdělit do samostatných celků nezávislých na jádře. 

Všechny tyto celky jsou v [[Procesor#Režimy procesoru|chráněném režimu]], zatímco jádro zůstává s těmi nejnutnějšími povinnostmi (správa procesů, správa paměti a meziprocesová komunikace) v [[Procesor#Režimy procesoru|režimu nechráněném]].

>[!info] Využití mikrojádra
Mikrojádra jsou v porovnání s monolitickými jádry pomalejší, ovšem své uplatnění našla v [[Embedded zařízení|embedded zařízeních]] a [[Systémy reálného času|v systémech reálného času]], jelikož zde často ani nejsou režimy procesoru, mezi kterými by se muselo přepínat, tudíž nemají takový výkonový handicap kvůli přepínání režimů.

>[!example] Schéma mikrojádra
>![[Pasted image 20230112024143.png]]

### Hybridní jádro
**Hybridní jádro** je architektura jádra, která se snaží zkombinovat výhody [[#Monolitické jádro|monolitického jádra]] (rychlost) a [[#Mikrojádro|mikrojádra]] (udržitelnost). Toho dosahuje tím, že některé služby nechá v [[Procesor#Režimy procesoru|prostoru jádra]], jiné zase přesune do [[Procesor#Režimy procesoru|uživatelského prostoru]].

[^1]:Roztříštění paměti, ke kterému dojde kvůli tomu, že souvislá část paměti není vyhrazena na startu operačního systému (jelikož nevíme, kolik jí budeme potřebovat)