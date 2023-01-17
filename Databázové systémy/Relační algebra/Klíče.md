Klíče je v [[Relační datový model|relačních databázích]] atribut, nebo kombinace atributů, která jednoznačně identifikuje $n$-tici relace (řádek tabulky).

## Kandidátní klíč
**Kandidátní klíč** je atribut nebo kombinace atributů, které jednoznačně identifikují $n$-tice a žádný atribut v nich není nadbytečný.

## Primární klíč
Primární klíč je konkrétní [[#Kandidátní klíč|kandidátní klíč]], který jsme zvolili jako nejvhodněji popisující dané řádky tabulky ($n$-tice relace).

Pokud nechceme používat [[#Kandidátní klíč|kandidátní klíč]], lze vytvořit **umělý primární klíč**
>[!faq] Co je to umělý primární klíč?
>**Umělý primární klíč** je takový klíč, který není tvořen atributy z relace.
>Zpravidla jde číslo, které začíná na 1 a s každým záznamem se přičítá 1.

>[!tip] Značení primárních klíčů ve schématu relace
>Pokud máme relaci $R(A_1, A_2, A_3, ...)$, pak poté primární klíč značíme <ins>podržením</ins>
>
>*Např.* $R(\underline{A_1}, A_2, A_3,\, ...)$

## Cizí klíč
Cizí klíč je atribut, který reprezentuje [[#Primární klíč|primární klíč]] jiné relace (tabulky).