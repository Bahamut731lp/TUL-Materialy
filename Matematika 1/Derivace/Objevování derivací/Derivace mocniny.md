Uvažujme o $y = x^2$. Celý diferenciální počet je o tom, že hledáme poměr růstu mezi dvěma proměnnými. V tomhle případě nás zajímá, jak rychle se mění $y$ v závislosti na $x$. Jinak řečeno, jaký je poměr $\frac{dy}{dx}$

 Nechme $x$ se trochu zvětšit, takže se z něho stane $x + dx$. Poté se zákonitě musí také zvětšit $y$, a to na $y + dy$. 
 $$
 \Large \begin{aligned}
 y &= x^2 \\ 
 &\downarrow \\
 y + dy &= (x + dx)^2 \\
 y + dy &= x^2 + 2x \cdot dx + (dx)^2 
 \end{aligned}
 $$
 Když se podíváme na upravenou rovnici, tak vidíme, že máme $x^2$, člen s malou změnou $2x\cdot dx$ a člen malé změny, která je ještě změněna o malou změnu - $(dx)^2$. Ten poslední člen můžeme bezpečně zahodit, protože změna změny nás úplně nezajímá, když už máme změnu jako takovou v členu $2x\cdot dx$.

$$
 \Large \begin{aligned}
 y + dy &= x^2 + 2x \cdot dx + \cancel{(dx)^2} \\ 
 &\downarrow \\
 y + dy &= x^2 + 2x \cdot dx 
 \end{aligned}
 $$
Pokud budem pokračovat v úpravách dál, abychom našli náš žádáný poměr, tedy ak moc roste $y$ v závislosti na $x$. Abychom se zbavili $y$, tak využijeme toho, e $y = x^2$:
$$
 \Large \begin{aligned}
 y + dy &= x^2 + 2x \cdot dx\\
 &\downarrow \\
 x^2 + dy &= x^2 + 2x \cdot dx &&\text{/}-x^2 \\
 dy &= 2x \cdot dx &&\text{/}\normalsize\frac{1}{dx} \\

 \Aboxed{\frac{dy}{dx} &= 2x}
 \end{aligned}
$$

Tomuhle postupu se říká derivování funkce ($y$) podle proměnné $x$. Derivace není nic jiného než nalezení tohodle poměru. Nikdo to takhle zdlouhavě nepočítá, proto se používá pravidlo pro derivování mocnin, které by nám od hnedka z místa dalo tenhle výsledek.
