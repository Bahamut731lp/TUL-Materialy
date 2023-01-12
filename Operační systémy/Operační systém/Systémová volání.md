**Systémové volání** je mechanismus, kdy [[Proces|proces]] z [[Procesor#Režimy procesoru|chráněného režimu]] požaduje po [[Operační systém|operačním systému]], aby za něj vykonal operaci v [[Procesor#Režimy procesoru|nechráněném režimu]]. 

>[!faq] Jak proces volá operační systém?
> Proces volá funkci z API operačního systému, která pod pokličkou vytváří požadavek na systémové volání. To je vytvořeno vyvoláním [[Přerušení#Softwarové přerušení|softwarového přerušení]], kde [[Přerušení#Tabulka přerušení|vektorem přerušení]] je patřičné systémové volání.

