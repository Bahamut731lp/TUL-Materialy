# Vektorové prostory
Vektorový (nebo též lineární) prostor nad [[Algebraické těleso|tělesem]] je množina, která má vyznačený nulový prvek a dvě binární operace - sčítání a násobení, pro které platí [[#Axiómy vektorového prostoru]].


---
Vektorový prostor je množina [[Vektor|vektorů]], pro kterou jsou určena nějaká pravidla. Aby mohl vektorový prostor existovat, musí být dána
- Neprázdná [[Množiny|množina]] $\large V$, jejíž prvky nazýváme **vektory**
- [[Algebraické těleso]] $\large T$
- [[Zobrazení]] $\large \oplus :\ V\times V\to V$ (**sčítání vektorů**)
- [[Zobrazení]] $\large \odot :\ T\times V\to V$ (**Násobení vektorů** prvkem z tělesa $\large T$)

Vektorový prostor tedy existuje, pokud máme neprázdnou množinu [[Uzavřenost množiny na operaci|uzavřenou na operace]] **sčítání** a **násobení** vektorů. 

Pravidla pro existenci a práci s vektorovými prostory se nazývají [[#Axiómy vektorového prostoru]], a jsou formálně velmi podobné [[Algebraické těleso#Axiómy tělesa|axiómům tělesa]]. Rozdíl je ale v tom, že operace v tělese a operace ve vektorovém prostoru **nejsou jedno a to samé**, jedná se totiž o různá zobrazení

---
## Axiómy vektorového prostoru
1. **Komutativnost sčítání vektorů** - Pro libovolné vektory $a, b$ z vektorového prostoru $V$ musí platit, že:
	1. $a \oplus b = b \oplus a$
2. **Asociativita sčítání vektorů** - Pro libovolné vektory $a, b$ z vektorového prostoru $V$ musí platit, že:
	1. $a \oplus (b \oplus c) = (a \oplus b) \oplus c$
3. **Existuje nulový vektor** - Ve vektorovém prostoru existuje vektor, který si označíme jako $0$ , pro který platí, že:
	1. $a \oplus 0 = a$
4. **Existuje opačný vektor** - Pro libovolný vektor $a$ musí existovat opačný vektor $-a$, pro které platí, že:
	1. $a \oplus -a = 0$
5. **Existuje jednotkový vektor** - Existuje prvek, který si označíme jako $1$, pro který platí, že:
	1. $a\cdot 1=a$
6. **Distributivnost** - Distributivnost platí vzhledem ke sčítání prvků tělesa a i ke sčítání vektorů
	1. $(a \oplus b )\odot c = (a \odot c) \oplus (b \odot c)$
7. **Netrivialita** - Nulový prvek a jednotkový prvek **nesmí** být stejné
	1. $0\not=1$

