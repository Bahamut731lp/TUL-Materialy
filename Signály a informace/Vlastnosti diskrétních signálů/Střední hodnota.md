Střední hodnota signálu je číslo, které vyjadřuje průměrnou hodnotu signálu.

>[!tldr]
>- Jedná se o jistou formu průměru signálu
>- Lze měřit pouze na konečných a periodických signálech[^1].

$$\Large \overline{X} = \frac{1}{N}\sum_{i=0}^{N - 1}x[i]$$

[^1]: Techninky vzato by střední hodnota šla realizovat na nekonečných signálech, protože se jedná o průměr, šlo by využít vztahu $X_{new} = X_{old} + \frac{x - X_{old}}{N}$, kde $N$ je počet vzorků včetně aktuálního... tento postup je ale docela nepraktickej, proto se to moc nedělá.