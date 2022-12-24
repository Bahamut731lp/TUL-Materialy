- Slouží k omezení přístupu na ty data, na které musí uživatel vidět.
- Zabraňují škodlivým modifikacím dat

[[Autorizační identifikátor]]

- Práva jsou povolené akce nad [[Relace|relacemi]].
- CRUD operace
- Přidávání práv pomocí příkazu `GRANT`
- Lze přidat `WITH GRANT OPTION`, který dovolí předávat stejná nebo menší práva dalším uživatelům
- Odebrání práv přes `REVOKE`
- Odebrání i dalším přes `CASCADE`, nebo `RESTRICT`

**Příklad:**
```sql
UPDATE prihlasky
SET rozhodnuti = 'Y'
WHERE uJmeno = 'TUL' and sID IN (SELECT sId FROM Studenti WHERE prumer < 2.0)
```

Potřebuje `UPDATE(rozhodnuti)`, `SELECT(uJmeno, sId)`