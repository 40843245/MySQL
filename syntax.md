# MySQL
## syntax
### `EXISTS` clause

```
<field> EXISTS [<table>|<subquery>]
```

### `NOT EXISTS` clause

```
<field> NOT EXISTS [<table>|<subquery>]
```

> [!CAUTION]
> `NOT EXISTS` clause is opposite of `EXISTS` clause.

For more details about `EXISTS` clause and `NOT` clause that used in subquery, see [`Subqueries with EXISTS or NOT EXISTS` MySQL official docs](https://dev.mysql.com/doc/refman/8.4/en/exists-and-not-exists-subqueries.html)

### subquery
A subquery refers the an other query in a query.

#### type of subquery according indpendence of outer query
##### self-contained subquery
`outer query` does NOT relate to `inner query`.

##### correlated subquery
`outer query` relates to `inner query`.

#### type of subquery according to returned value or table.
##### subquery with returned single value
`inner query` returns a table with only single value (a table of one row, one column).

For example, `inner query` is 

`SELECT MAX(emp.sal) FROM emp;`

| MAX(sal) |
| :- |
| 1500 |

##### subquery with returned multiple values
`inner query` returns a table with only multiple values but one field (a table of many rows, one column).

For example, `inner query` is

`SELECT emp.ename FROM emp GROUP BY emp.sal;`

| emp.ename |
| :- |
| SMITH |
| CLERK |
| BILL |

##### subquery with returned multiple fields
`inner query` returns a table with only one value but many field (a table of one row, many columns).

For example, `inner query` is

`SELECT emp.ename, emp.sal FROM emp WHERE emp.name = 'SMITH';`

| emp.ename | emp.sal |
| :- | :- |
| SMITH | 2000 |

##### subquery with returned table
`inner query` returns a table (a table of many columns, many columns).

For example, `inner query` is

`SELECT emp.ename, emp.sal FROM emp GROUP BY emp.sal;`

| emp.ename | emp.sal |
| :- | :- |
| SMITH | 2000 |
| CLERK | 2000 |
| BILL | 2500 |


### `WITH` clause
#### syntax 

```
with_clause:
    WITH [RECURSIVE]
        cte_name [(col_name [, col_name] ...)] AS (subquery)
        [, cte_name [(col_name [, col_name] ...)] AS (subquery)] ..
```

For more details, see `WITH` clause[^1]

### CTE (Common Table Expression)

> [!IMPORTANT]
> To specify CTE, use a `WITH` clause that has one or more comma-separated subclauses.
>
> Each subclause provides a subquery that produces a result set, and associates a name with the subquery. 

CTE is defined with `WITH` clause.
For syntax, see [`WITH` clause](#syntax-1)

### Recursive CTE (Recursive Common Table Expression)
CTE is defined with `WITH` clause followed by `RECURSIVE` clause.

As following example:

```
WITH RECURSIVE cte (n) AS
(
  SELECT 1
  UNION ALL
  SELECT n + 1 FROM cte WHERE n < 5
)
SELECT * FROM cte;
```

## footnotes
[^1]: [`WITH` clause (MySQL official website)](https://dev.mysql.com/doc/refman/8.4/en/with.html)
