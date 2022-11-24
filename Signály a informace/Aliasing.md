**Aliasing** (neboli ***překládání frekvencí***) je jev, který vzniká při vzorkování signálu, který má frekvenci nad polovinou [[Vzorkovací frekvence|vzorkovací frekvence]]. Jinak řečeno, překládání frekvencí vzniká při nedodržení vzorkovacího teorému.

[[Číslicová frekvence|číslicová]] kosinusovka nemusí být vždy periodická. 
> TODO: Doplnit vzorečky


$$\large
\begin{aligned}
	f_a &= f - kf_s \\
	f_a &\in \left(-\frac{1}{2}f_s, +\frac{1}{2}f_s\right)
\end{aligned}
$$

## Antialiasing
Před A/D převodem se signál prožene antialiasingovým filtrem (dolní propust).