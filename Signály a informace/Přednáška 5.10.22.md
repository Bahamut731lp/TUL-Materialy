# Přednáška 5.10.22

Vznik číslicových signálů
- Převodem z analogových signálů
- Vytvoření posloupnosti vzorků z naměřených hodnot
- Vytvoření dat  nějakým generátorem

Často se bude pracovat s jednorozměrnými, nebo dvourozměrnými signály. Viz [[Signál]].

- Vytvoteřní číslicového signálu výčtem
```matlab
x = [ ... ]
plot(x) % Vytvoření spojitého grafu vzorků
stem(x) % Vytvoření nespojitých "stonků" grafu
```

- Vytvoření signálu navzorkováním funkce
```matlab
Fs = 100; % Vzorkovací frekvence
Ts = 1 / Fs; % Vzorkovací perioda

t = -1:Ts:1; % Vytvoření časové osy

% Vytvoření prvního signálu
f = 10;
x = sin(2*pi*f*t);

% Vytvoření druhého signálu
fm = 2;
y = sin(2*pi*fm*t);

% Součin signálu (Modulace amplitudy)
z = x .* y;
```
---
- Kvantizace - převod na menší počet úrovní
- Počet úrovní na barvu: $32 = 2^8$ bitů.
---

## Bonusová úloha
**Natočení obrázku**
TL,DR: Použít lin. regresi

```matlab
%obr = matice bodů
imread("cesta");
imrotate(obr, uhel);
imwrite(obr, cesta);
subplot(n, m) % Matice n * m v obrázku

```