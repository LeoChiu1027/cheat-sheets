
---
```SQL
SELECT
  nspname AS schemaname,
  relname,
  reltuples
FROM
  pg_class C
  LEFT JOIN pg_namespace N ON (N.oid = C.relnamespace)
WHERE
  nspname NOT IN ('pg_catalog', 'information_schema')
  AND relkind = 'r'
  and nspname in ('offchain_db')
ORDER BY
  relname asc;
```