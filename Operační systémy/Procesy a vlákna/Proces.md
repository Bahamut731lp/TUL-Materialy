Proces je spuštěný [[Program|program]], který je zaveden do operační paměti.

>[!faq] Co potřebuje proces?
>Proces je tvořen kódem, daty a zdroji
>![[Pasted image 20230112032347.png]]

>[!info] Data o procesu
>Data o procesu jsou záznamy, které si [[Operační systém|operační systém]] vede o daném procesu.
>- Tyto záznamy jsou uloženy v chráněné části paměti
>- Často se označuje jako *Process Control Block*

>[!info] Data procesu
>Data procesu jsou záznamy, které si proces vede ve své čásit paměti a s kterou pracuje.

## Stavy procesu

|Stav|Vysvětlení|
|:--:|:--:|
|Waiting (Ready)|Čekající na strojový čas CPU|
|Running|Má přidělený CPU a vykonává svůj kód|
|Blocked|Proces čeká na výsledky (IO)|

>[!example] Stavy procesů
>![[Pasted image 20230112034132.png]]