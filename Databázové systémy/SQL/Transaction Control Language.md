**Transaction Control Language** slouží ke správě transkací, které jsou prováděny nad[[Databázový objekt|databázovém objektem]].

```sql
COMMIT    -- Uloží výsledky transakce do databáze
ROLLBACK  -- Obnoví databázi do posledního konzistentního stavu
SAVEPOINT -- Vytvoří dočasný záchytný bod, do kterého lze ROLLBACKnout
```