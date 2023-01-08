**Aliasing** (neboli **překládání frekvencí**) je jev, který vzniká při vzorkování signálu, který je vzorkován frekvenčí menší než je dvojnásobek té nejvyšší frekvence. Jinak řečeno, překládání frekvencí vzniká při nedodržení [[Vzorkování signálu#Vzorkovací teorém|vzorkovacího teorému]].

[[Číslicová frekvence|číslicová]] kosinusovka nemusí být vždy periodická. 
> TODO: Doplnit vzorečky


$$\large
\begin{aligned}
	f_a &= \left|f - f_s\cdot\left\lfloor{\frac{2f+f_s}{2f_s}}\right\rfloor\right|
\end{aligned}
$$

## Antialiasing
Před A/D převodem se signál prožene antialiasingovým filtrem (dolní propust).