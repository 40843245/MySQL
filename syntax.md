# MySQL
## syntax
### CTE (Common Table Expression)
#### syntax 
CTE is defined with `WITH` clause.

```
with_clause:
    WITH [RECURSIVE]
        cte_name [(col_name [, col_name] ...)] AS (subquery)
        [, cte_name [(col_name [, col_name] ...)] AS (subquery)] ..
```

For more details, see[^1]

## footnotes
[^1]: [CTE (MySQL official website)](https://dev.mysql.com/doc/refman/8.4/en/with.html)
