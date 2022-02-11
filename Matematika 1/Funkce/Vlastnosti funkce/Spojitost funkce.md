# Spojitost funkce
Spojitost funkce říká, jestli je někde graf funkce "přerušený" nebo ne. Funkce je spojitá v nějakém bodě, pokud je spojitá i v jeho libovolném okolí větší než 0.

>**Definice spojitosti:**
>Funkce je spojitá v bodě $c$, jestliže pro $\varepsilon$-okolí bodu $f(c)$ existuje takové $\delta$-okolí bodu $c$, že všechny $x$ z $\delta$-okolí mají funkční hodnotu v $\varepsilon$-okolí.
>$$\Large\begin{aligned}
	>|f(x)-f(c)| &< \varepsilon \\
	>|x-c| &< \delta \\
\end{aligned}$$

Spojitost lze také zadefinovat pomocí [[Limita funkce|limity]].
>**Definice spojitosti:**
>Funkce je spojitá v bodě $c$, pokud má b vodě $c$ limitu rovnou funkční hodnotě v bodě $c$.
>$$\Large\lim_{x\to{c}}f(x) = f(c)$$

Pokud jsou dvě funkce spojité v nějakém bodě, tak pak budou spojité i jejich "aritmetické operace".

>**Spojitost aritmetiky funkcí:**
>Mějme dvě spojité funkce v bodě $c$, poté jsou také spojité následující operace:
>- Absolutní hodnoty
>- Součet funkcí
>- Rozdíl funkcí
>- Součin funkcí
>- Podíl funkcí, pokud je funkční hodnota v jmenovateli různá od nuly.

>**Spojitost složené funkce:**
>Mějme dvě funkce, kde první je spojitá v bodě $c$, a druhá je spojitá ve funkční hodnotě první funkce v bodě $c$, poté je jejich složená funkce také spojitá v bodě $c$.
>$$\Large\begin{cases}
>c \in \mathbb{R} &\large\text{Zkoumaný bod.}\\
>g(c) & \large\text{Vnitřní funkce spojitá v bodě c.} \\
>h(g(c)) &\large\text{Vnější funkce spojitá ve funkční hodnotě vnitřní funkce.}\\
>h(g) &\large\text{Složená funkce je spojitá.}
>\end{cases}$$

## Jednostranná spojitost
Spojitost lze zkoumat buďto 
- **zleva**, kde $\delta$-okolí je pouze od bodu doleva.
- **zprava**, kde $\delta$-okolí je pouze od bodu doprava.
- **zleva i zprava**, kde $\delta$-okolí zkoumám od bodu do obou směrů.

## Spojitost inverzní funkce
Pokud je výchozí funkce spojitá, a lze k ní vytvořit inverzi (to znamená, že je [[Prostost funkce|prostá]] $\iff$ [[Monotónnost funkce|ryze monotónní]]), tak bude spojitá i její inverze. Dává smysl, kde by se v ní, přece jenom, najednou vzaly díry?

>**Spojitost inverzní funkce**:
>Mějme funkci $f$, která je [[Monotónnost funkce|ryze monotónní]] a spojitá na vybraném intervalu. Poté bude inverzní funkce také spojitá na vybraném intervalu.