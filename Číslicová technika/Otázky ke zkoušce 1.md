# Otázky ke zkoušce

**1. Nakreslete zatěžovací charakteristiku invertoru TTL, vyznačte v ní významné hodnoty.**

|Logická hodnota|Vstup/Výstup|Rozsah|
|:--:|:--:|:--|
|0|Vstup|$0 - 0.8V$|
|1|Vstup|$2 - 5V$|
|0|Výstup|$0 - 0.4V$|
|1|Výstup|$2.4 - 4V$|

>**Logické úrovně TTL signálů**:
>
>![[Pasted image 20220606174229.png]]

>**Zatěžovací charakteristika:**
>
>![[TTL Invertor.png]]

**2. Moorův zákon**
[[Moorův zákon]] je empirické pravidlo, které říká, že se složitost součástek každý rok zdvojnásobí při zachování stejné ceny.

Rychlost růstu složitosti se postupně zpomaluje, dneska se složitost zdvojnásobí zhruba za 1.5 roku.

**3. BiCMOS technologie**
[[Tranzistory#BiCMOS tranzistory|BiCMOS tranzistory]] jsou tranzistory, které kombinují bipolární tranzistory a unipolární CMOS tranzistory.

Výhodou je vyšší rychlost než CMOS, menší úbytek napětí než u bipolárních tranzistorů, flexibilní I/O (protože můžeme používat TTL či CMOS) a odolnost vůči mikropřírazům *(latch-up)*. Nevýhodou je vyšší cena a složitost výroby. Nejčastěji se používají ve vysokofrekvenčních zesilovačích.

**4. Vysvětlení s-term, p-term, minterm, maxterm**
(viz [[Booleovský výraz]])

>Vysvětlení termínů
>
>|Termín|Popis|
|:--|:--|
|**Term**|Výraz tvořený pouze proměnnými v log. součtu nebo součinu|
|**P-Term**|Term pouze s operací součinu|
|**S-Term**|Term pouze s operací součtu|
|**Minterm**|P-Term obsahující všechny nezávislé proměnné|
|**Maxterm**|S-Term obsahující všechny nezávislé proměnné|

**5. Kdy nastane přetečení u binární sčítačky**
(viz [[Přetečení]])

Přetečení nastane, když při součtu dvou kladných čísel výjde záporné a naopak.

**6. Základní bloky FPGA, čím se liší od CPLD, PLD**
- PLD - Pevně dané struktury (AND pole, OR výstupy)
- CPLD - Vícero GAL bloků, které jsou propojeny makrobuňkami a propojovací maticí
- FPGA - Maticové uspořádání programovatelných bloků

FPGA mývá již zabudované základní obvodu, jako jsou např. hodiny či řadiče periferií. FPGA obsahuje programovatelné CLB bloky s LUT.

**7. Nakreslete principielní schéma dekodéru z bin kódu 1 z 5 **
Tohle je pěkně stupidní zadání, na který bych se musel zeptat, jak to vlastně myslí.

>**Vstupy:**
>
>|S|$A_1$|$A_2$|$A_3$|$A_4$|$A_5$|
|:--:|:--:|:--:|:--:|:--:|:--:|
|**0**|0|0|0|0|1|
|**1**|0|0|0|1|0|
|**2**|0|0|1|0|0|
|**3**|0|1|0|0|0|
|**4**|1|0|0|0|0|
>
>**Výstupy:**
>
>|**S**|$Z_1$|$Z_2$|$Z_3$|
|:--:|:--:|:--:|:--:|
|**0**|0|0|1|
|**1**|0|1|0|
|**2**|0|1|1|
|**3**|1|0|0|
|**4**|1|0|1|
>
>$Z_1=\overline{A_1}A_2\overline{A_3A_4A_5}+A_1\overline{A_2A_3A_4A_5}$
>$Z_2=\overline{A_1A_2A_3}A_4\overline{A_5}+\overline{A_1A_2}A_3\overline{A_4A_5}$
>$Z_3=\overline{A_1A_2}A_3\overline{A_4A_5}+A_1\overline{A_2A_3A_4A_5}$

![[Pasted image 20220606203305.png]]

**8. Obvody s třetím stavem, k čemu se používají? Schéma?**
Třetím stavem se myslí stav **vysoké impedance** (odpojení vodiče). Používá se, pokud potřebujeme odstranit vliv zařízení z obvodu (a nebo zamezení zkratu). Třístavové obvody jsou základem sběrnic.

**9. Rozlišení klopných obvodů podle spínání**
- Obvody reagující na **náběžnou hranu**
- Obvody reagující na **sestupnou hranu**
- Obvody reagující na **náběžnou i sestupnou hranu** (hladinu)

**10. Popiště obvod na obrázku**
Obvod na obrázku je D-Latch, což je v podstatě jednobitová pamět.
> ![[Pasted image 20220606203807.png]]

**11. Co je za obvod na obrázku?**
Obvod na obrázku je přímo mapovaná cache. Adresa přivedena na dekodér, ten vybere řádek z tabulky, tagy se pak porovnají v komparátoru $\implies$ rozhodnutí, zda tam data jsou, či ne.
>![[Pasted image 20220606205155.png]]

**12. Popiště algoritmus Quine-McCluskey**
(viz [[Minimalizace Quine-McCluskey]])

**13. Navrhněte dekodér pro 7-segmentový displej z kódu BCD**
(viz [[Měření 4]])

**14. Navrhněte synchronní sekvenční obvod bla bla bla**

**15. idk**

**16. Co je to maxterm?**
(viz [[Booleovský výraz]])

Maxterm je s-term (výraz skládájící se z přímých či negovaných proměnných pouze v logickém součtu), který obsahuje všechny nezávislé proměnné, např.

$$\large F(a, b, c, d) = a+\overline{b}+c+\overline{d}$$

**17. Navrhněte obvod realizující prahovou funkci s prahem $\text{0B}_H$ ze čtyř proměnných v UNDF**
- Prahová funkce = Funkce, která vrací jedničku až po překročení určitého prahu
- UNDF = Součet všech mintermů

**18. Jaký je rozdíl mezi jednoportovou a dvouportovou pamětí?**
- **Jednoportová paměť** má jednu adresní sběrnici a vstup, který určuje operaci (čtení/zápis)
- **Dvouportová paměť** má dva nezávislé paměťové obvody (se svými adresními a datovými sběrnicemi včetně řídících signálů)

**19.  Co je to faktorizace obvodu?**

**20. Jaké jsou základní rozdíly mezi ECL a CMOS?**

**21. Nakreslete schéma 4 bitového synchronního čítače s paralelním přenosem**
(viz cvika)

**22. Jaký obvod je na obrázku? Jaké je maximální zpoždění signálu, které může v obvodu nastat?**
- Obvod kontrolující paritu (počet lichých jedniček).
- Zpoždění bude $n\cdot\text{zpoždění XOR hradla}$

>![[Pasted image 20220606232915.png]]

**23. Jaký obvod je na obrázku?**
- Na obrázku je jednobitová sčítačka, která je tvořená polosčítačkama.
- Obvod realizuje součet jednobitových čísel

>![[Pasted image 20220606233121.png]]

**24. Uveď posloupnost stavů procesoru, kterými prochází při provádění instrukce**
Zobecněný instrukční cyklus je následující:
1. Načtení instrukce
2. Dekódování instrukce
3. Načtení operandů
4. Provedení instrukce
5. Zapsání výsledků

**25. Co je to logický zdvih? Je tato veličina využitelná k popisu vlastnostností CMOS log. obvodů?**
- Pásmo zakázaných napěťových úrovní mezi logickou nulou a jedničkou.
- Ano, protože čím větší je toto pásmo, tím se obvod považuje za bezpečnější z hlediska rozpoznávání logických úrovní (hůře se mu plete logická nula a jedna).

**26. Co je to dynamický hazard a jak vzniká?**
(viz [[Hazardy]])
- Dynamický hazard je vícenásobná neočekávaná změna výstupní hodnoty obvodu.
- Jedná se o kaskádový efekt pramenícího z jednoho či více statických hazardů.

**27. Co je to statický hazard a jak vzniká?**
- Statický hazard je neočekávaná změna výstupní hodnoty obvodu
- Vzniká různými rychlostmi šíření signálu ve větvích, které se následně spojují do jedné.

**28. Je možné převést automat typu Moore na Mealy tak, aby měli stejnou funkci?**
- Ano, pokud mají stejné vstupy/výstupy.
- Jediný rozdíl je v tom, že Moore má o jeden stav více (Mealy výstup posílá okamžitě, Moore až o "takt" později)

**29. Nakreslete Johnsonův čítač. Kolik stavů generuje?**
- Generuje $2n$ stavů

>![[Pasted image 20220606235846.png]]

**30. Co je to logický zisk?**
Logický zisk je počet vstupů připojených na jeden výstup. Maximální počet připojitelných vstupů se uvádí v tabulkách (U TLL zpravidla 10)

**31. Nakreslete sčítačku-odčítačku v doplňkovém kódu**
>![[Pasted image 20220607001247.png]]

**32. Nakreslete převodní charakteristiku CMOS invertoru**
> ![[Pasted image 20220607001411.png]]

**33. Jaký je rozdíl mezi zakázkovými a programovatelnými ASIC procesory?**
- **Programovatelné** si může zákazník upravit sám
- **Zakázkové** jsou vyráběne pro konkrétní účel a jsou pro něj také optimalizované

**34. Popiště funkci liché parity pro 3 proměnné pomocí UNDF a UNKF**
- Lichá parita: 1 když má funkce lichý počet jedniček
- UNDF: Úplná normální disjunktní forma
- UNKF: Úplná normální konjuktivní forma

**35.  Jaká jsou kritéria minimality logických výrazů?**
- Co nejméně [[Booleovský výraz|termů]]
- Co nejméně nezávislých proměnných v [[Booleovský výraz|termu]]
- Co nejméně negací

**36. Co je to kombinační obvod?**
(viz [[Kombinační obvody]])
- Kombinační obvod je takový obvod, jehož výstup závisí jen a pouze na okamžitém stavu vstupu.

**37. Co je CLB a LUT**
(viz [[FPGA]])
- CLB (Configurable Logic Block) - Programovatelná buňka v FPGA obvodech
- LUT (Lookup Table) - Blok realizující pravdivostní tabulku uvnitř FPGA buněk.

**38.  Schéma 2 bitového posuvného registru  s možností přepínání mezi sériovým a paralelním režimem**

>Něco podobného tomuhle, jenom se musí doplnit ovládací logika na přepínání sériového a paralelního režimu
>
>![[Pasted image 20220607213347.png]]

**39. Co je to přímý implikant logické funkce?**
- Přímý implikant je takový term, který po vynechání proměnné přestává implikovat logickou danou logickou funkci

**40. Nakreslete odběrovou charakteristiku TTL invertoru**

>**Odběrová charakteristika TTL invertoru**
>
>![[Pasted image 20220607221045.png]]

**41. Jaký mají význam časy T-Set a T-Hold ve vícestupňových klopných obvodech?**
- Jedná se o časy, které udávají, po jakou dobu musí být data stabilní (neměnná)
- **T-Set** je doba před hranou hodinového signálu
- **T-Hold** je doba po hraně hodinového signálu

>**Diagram ukazující T-Set a T-Hold**
>
>![[Pasted image 20220607221317.png]]

**42. Co je to plně asociativní cache?**
Celá adresa je brána jako tag, tudíž má kažý řádek tabulky vlastní komparátor

>**Plně asociativní cache**
>
>![[Pasted image 20220608075158.png]]

**43. Popiště, jakým způsobem pracuje násobička**

>**Násobička**
>
>![[Pasted image 20220608075513.png]]
