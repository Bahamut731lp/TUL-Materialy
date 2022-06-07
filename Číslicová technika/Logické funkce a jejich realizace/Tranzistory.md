# Tranzistory
Třívodičová součástka, která se používá jako přepínač.

## Bipolární tranzistor
Bipolární tranzistory jsou tranzistory tvořené třemi vrstvami polovodiče, které tvoří dva **přechody PN**. Bipolární tranzistory se používají jako zesilovače, spínače nebo invertory.

![[Pasted image 20220606153750.png]]

### Tranzistorový jev
Bipolární tranzistory se staly populární součástkou díky **tranzistorovému jevu**, který ve zkratce říká, že pomocí menšího proudu jsme schopni ovládat průchod většího proudu.

![[Pasted image 20220606151015.png]]

## Unipolární tranzistory
Unipolární tranzistory používají exkluzivně jenom [[Polovodič#P-Typ|děrovou vodivost]], nebo [[Polovodič#N-Typ|elektronovou vodivost]][^1].


## MOS (Metal Oxide Silicon) Tranzistory
Jedná se o součástku, az kterých se vyrábí polosilikonová nebo kovová hradla. Podle typu použitého polovodiče mají různé vlastnosti:

|Tranzistor|Typ polovodiče|V okolí logické nuly|V okolí logické jedničky|
|:--:|:--:|:--:|:--:|
|nMOS|N|Dobrá vodivost|Vyšší úbytek napětí|
|pMOS|P|Vyšší úbytek napětí|Dobrá vodivost|

MOS tranzistory mají tři vývody:
- **Source** (zdroj), který slouží jako vstup/výstup pro řízený proud
- **Drain** (odtok), který slouží jako vstup/výstup pro řízený proud
- **Gate** (brána), který slouží pro ovládání proudu procházející tranzistorem

|Tranzistor|Gate = 0|Gate = 1|
|:--:|:--:|:--:|
|nMOS|0|1|
|pMOS|1|0|

## CMOS (Complementary MOS) tranzistory
CMOS tranzistory jsou tranzistory, které dva MOS tranzistory 
- jeden **pMOS**,
- a jeden **nMOS**

CMOS tranzistory spoléhají na stavovou symetrii těchto tranzistorů, to znamená, že když je jeden sepnutý, druhý je rozepnutý, a naopak. Jejich výhodou je nulová klidová (idle) spotřeba a větší hustotu integrace.

Nevýhodou je, že CMOS hradla bývají zpravidla omezeny pouze na 2 vstupy. To lze samozřejmě obejít kaskádovým zapojením několika hradel.


## BiCMOS tranzistory
BiCMOS tranzistory jsou tvořeny [[#Bipolární tranzistor|bipolárním tranzistorem]] v kombinaci s [[#CMOS Complementary MOS tranzistory|CMOS tranzistorem]].

Tyto tranzistory nabízí vyšší rychlost než CMOS, menší úbytek napětí než u bipolárních tranzistorů, flexibilní I/O (protože můžeme používat TTL či CMOS) a odolnost vůči mikropřírazům *(latch-up)*[^2]

[^1]: Obě dvě varianty najednou používají právě bipolární tranzistory
[^2]: Mikropřírazy jsou jev, který vzniká při překročení maximálního rozsahu napájecího napětí. Způsobuje vytvoření zkratu, který parazituje vstupní napětí takovým způsobem, že se skoro žádné nedostane do původního hradla.