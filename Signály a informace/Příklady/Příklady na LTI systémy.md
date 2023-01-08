Uvažuje systém $2y[n] = x[n] + 3x[n-2] + y[n-1]$, zjistěte modul $|H(f)|$ a fázi $\varphi(F)$ stejnosměrné složky.

$2y[n] - y[n-1] = x[n] + 3x[n-2] \to H(z) = \frac{1 - 3z^{-2}}{2-z^{-1}}$

$z^{n} = e^{2\pi{F}{n}j}$

$\large H(F) = \frac{1 - 3e^{-4\pi{F}j}}{2 - e^{-2\pi{F}j}}$

Modul stejnosměrné složky:
$\large |H(0)| = |\frac{1 - 3e^{0}}{2 - e^{0}}| = |\frac{-2}{1}| = \boxed{2}$

Fáze stejnosměrné složky:
$e^{-4\pi{F} + 2\pi{F}} = 2\pi{F} = \boxed{0}$

