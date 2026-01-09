# SQL SERVER


### Triggers
```sql
-- list triggers
SELECT t.name AS TriggerName
FROM sys.triggers t
JOIN sys.tables tb ON t.parent_id = tb.object_id
WHERE tb.name = 'TABLE_NAME';
```

### Tables
```sql
-- Gets all column names from a table as a single comma-separated list.
SELECT STRING_AGG(name, ', ') AS ColumnList
FROM sys.columns
WHERE object_id = OBJECT_ID('TABLE_NAME')
```

