Pohled je virtuální relace (tabulka), která se používá pro skrytí části dat, resp. výběru "jen těch potřebných".

**Materializovaný pohled**: ...

```sql
CREATE VIEW jmeno as (
	-- SQL Dotaz
)

DROP VIEW jmeno
```

## Modifikace dat z pohledu
Lze buďto omezit, nebo definovat, co dělat přes trigger. Důležité povolit jenom modifikace, které jsou vidět v pohledu.