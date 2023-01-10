Backtracking je metoda pro vytváření [[Algoritmizace a programování 1/Základy/Algoritmus|algoritmu]], který [[Brute Force|hrubou silou]] hledá taková řešení, která odpovídají našim požadavkům.

Backtracking se dá uplatnit na úlohy, na které jsou kladena jistá omezení. Pomocí [[Algoritmizace a datové struktury/Rekurze/Rekurze|rekurze]] vytváří [[Strom|strom]], kde každá větev reprezentuje proměnnou a každá úroveň reprezentuje řešení.

Backtracking nám pak může pomoct nalézt:
- Možné řešení
- Nejlepší řešení
- Všechna možná řešení

>[!example]- Problém sousedících barev
>Představte si situaci, kdy máte na $n\cdot m$ ploše rozmístěno $x$ bodů.
>- Každý bod má náhodné souřadnice
>- Každý bod má unikátní souřadnice ($\forall n, m: [n_1, m_1] \not= [n_2, m_2]$)
>- Každý bod má kromě souřadnic přiřazenou také barvu.
>
>Naším úkolem je udělat takový algoritmus, který najde takové řešení, ve kterém platí, že všechny sousedící barvy...

>[!example]- Problém osmi dam