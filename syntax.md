# MySQL
## syntax
### CTE (Common Table Expression)

#### syntax 
CTE is defined with `WITH` clause.

See [`WITH` clause](#syntax-1)

For more details, see `WITH` clause[^1]

### `WITH` clause
#### syntax 

```
with_clause:
    WITH [RECURSIVE]
        cte_name [(col_name [, col_name] ...)] AS (subquery)
        [, cte_name [(col_name [, col_name] ...)] AS (subquery)] ..
```

For more details, see `WITH` clause[^1]

## footnotes
[^1]: [`WITH` clause (MySQL official website)](https://dev.mysql.com/doc/refman/8.4/en/with.html)
