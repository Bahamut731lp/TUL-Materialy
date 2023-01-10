**Algoritmus Knuth-Morris-Pratt** je algoritmus pro prohledávání řetězců, který staví na [[Přirozené prohledávání|přirozeném prohledávání]] a chytrém řízení posunu.

Hledaný největší možný posun je roven  délce největšího prefixu P[0:j-1], který je  
suffixem P[1:j-1].

Celou analýzu prefixů a suffixů lze provést předem, poté Chybová funkce (failure function) F(k)je  definována jako nejdelší prefix P[0:k], který je také suffixem P[1:k].