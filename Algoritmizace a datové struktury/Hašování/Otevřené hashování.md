**Otevřené [[Hashovací funkce|hashování]]** je mechanismus řešení kolizí, ve kterém je tabulka adres uložená do pole, a při kolizi se nějakou metodou prohledávají další prvky pole, dokud se nenajde prázdná pozice.

Proces hledání volné pozice se nazývá **probing**.

## Linear Probing
**Linear Probing** je proces hledání volného místa tím, že se lineární vyhledává nejbližší volná pozice.

## Double Hashing
Double Hashing používá místo lineárního prohledávání druhou hashovací funkci k nalezení volné pozice.