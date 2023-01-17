**Transakce** označuje souvislou [[Matematika 1/Posloupnosti/Posloupnosti|posloupnost]] [[SQL|příkazů]], která převádí databázi z jednoho konzistentního stavu do druhého.

>[!tldr]
>- Transakce řídí přechod z jednoho konzistentního stavu do druhého
>- Zapouzdřují posloupnost příkazů do jednoho bloku
>- Umožňují nezávislý přístup více uživatelům naráz
>- Vytvářejí odolnost vůči poruchám

## Autocommit
- Při zapnutém režimu `auto_commit` je každý [[SQL|příkaz]] brán jako samostatná transakce
- Při vypnutém režimu `auto_commit` se musí 
	- manuálně začít transakce (např. `BEGIN TRANSACTION`)
	- manuálně ukončit transakce (např. `COMMIT` nebo `ROLLBACK`)

## Vlastnosti transakcí
>[!tip] Atomicita
>- Transakce se tváří jako jeden celek a takto tak pracuje.
>- Buďto se provede celá, a nebo vůbec.

>[!tip] Konzistence
>- Transakce převádí [[Databázové systémy|databázový systém]] z jednoho konzistentního stavu do druhého

>[!tip] Izolovanost
>- Každá transakce je izolovaná a nemůže pracovat s dílčimi efekty jiných transakcí.

>[!tip] Trvanlivost
>Úspěšná transakce je uložena do databáze

## Serializovatelnost
- Současné vykonávání transakcí nesmí zapříčinit selhání programu
- Lze zajistit [[Mutex|zámky]], ale transakce musí být rychlé, aby nezdržovaly.
- Lze nastavit různé úrovně izolovanosti transakce, čímž lze ovlivnit, jak moc zajistí konzistenci.