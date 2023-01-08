Přenosová funkce vyjadřuje poměr mezi vstupní a výstupní funkcí [[LTI systém|LTI systémů]].

>[!tldr]
>- Přenosová funkce je podíl vstupní a výstupní funkce v [[Laplaceova transformace|Laplaceově transformaci]]
>- Přenosová funkce [[LTI systém|LTI systému]] je ve tvaru $H(z) = \frac{B_0z^0 + B_1z^{-1}+...}{A_0z^0 + A_1z^{-1}+...}$
>- Členy v čitateli jsou **nuly**
>- Členy v jmenovateli jsou **póly**


Komplexní proměnná $z^-1$ má význam jednotkového zpoždění. Analogicky $z^{-n}$ je zpoždění o $n$ vzorků. 

## Převod z diferenční rovnice na přenosovou funkci
>[!example] Nalezněte přenosovou funkci systému zadaného pomocí diferenční rovnice
>$$\Large{y[n] = x[n]+2x[n-2]+2y[n-2]}$$

Nejdříve rovnici upravíme tak, abychom měli oddělené vstupy ($x$) a výstupy $y$:

$$y[n] - 2y[n-2] = x[n] + 2x[n-2]$$

Nyní si stačí vypsat koeficienty *nul* a *pólů*:
$$
\begin{aligned}
	x[n - 0] + 2x[n - 2] &= 1\cdot{z^{-0}}+2\cdot{z^{-2}} \\
	y[n - 0] - 2y[n - 2] &= 1\cdot{z^{-0}}-2\cdot{z^{-2}} \\
\end{aligned}
$$

Po menší úpravě a dosazení dostáváme přenosovou funkci:
$$\boxed{H(z) = \frac{1 + 2z^{-2}}{1 - 2z^{-2}}}$$

## Převod z přenosové funkce na diferenční rovnici