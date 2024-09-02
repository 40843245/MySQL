# MySQL
## basic clause
### database
#### `CREATE DATABASE`
To create a database, use `CREATE DATABASE` clause.

```
CREATE DATABASE <databaseName>;
```

See[`CREATE DATABASE` MySQL official docs](https://dev.mysql.com/doc/refman/8.4/en/creating-database.html)

#### `USE DATABASE`
To use the database as current database, use `USE` clause.

```
USE <databaseName>;
```

See[`CREATE DATABASE` MySQL official docs](https://dev.mysql.com/doc/refman/8.4/en/creating-database.html)

### table
#### `CREATE TABLE`
To create a new table, use `CREATE TABLE` clause.

```
CREATE TABLE <tableName>(
    <field>
    [,<field>]
);
```

where

```
<field> := <fieldName> <fieldType> <fieldModifiers>
```

See [`CREATE TABLE` MySQL official docs](https://dev.mysql.com/doc/refman/8.4/en/create-table.html)

#### `DROP TABLE`
See [`DROP TABLE` MySQL official docs](https://dev.mysql.com/doc/refman/8.0/en/drop-table.html)

#### `ALTER TABLE`
See [`ALTER TABLE` MySQL official docs](https://dev.mysql.com/doc/refman/8.0/en/alter-table.html)

### records in table
#### `SELECT`
The `SELECT` clause to select and display a variable or a table.

See [`SELECT` MySQL official docs](https://dev.mysql.com/doc/refman/8.0/en/select.html)

#### `INSERT`
To insert into data as rows in table, use `INSERT INTO` clause.

See [`INSERT` MySQL official docs](https://dev.mysql.com/doc/refman/8.0/en/insert.html)

#### `UPDATE`
To update one or more specific columns in table to new value, use `UPDATE` clause.

See [`UPDATE` MySQL official docs](https://dev.mysql.com/doc/refman/8.0/en/update.html)

#### `DELETE`
To delete one or more records in table which satisfies the condition followed by `WHERE` clause, use `DELETRE`. 

> [!CAUTION]
> If `WHERE` and its condition are omitted, it means `WHERE 1` which will delete all records. Very be careful about that.

> [!CAUTION]
> In MySQL, to prevent to update and delete more records accidently. Execute the MySQL command `SQL_SAFE_UPDATES` before updating or deleting.


#### `WHERE`
To filter out by given condition, use `WHERE` clause.

```
WHERE <condition1>
```

A query will only return datas that the `<condition1>` is evaluated to true.

See [`SELECT` MySQL official docs](https://dev.mysql.com/doc/refman/8.0/en/select.html)

##### `FROM`
To indicate the datas that we manipulate from the table or the returned value subquery (P.S. we can consider the returned value of a subquery as a table), use `FROM` clause.

See [`SELECT` MySQL official docs](https://dev.mysql.com/doc/refman/8.0/en/select.html)

##### `GROUP BY`
The clause `GROUP BY` groups the records with given fields.

```
GROUP BY <fieldName>
```

##### `HAVING`
To filter out with given conidition after grouping (using `GROUP BY` clause), use `HAVING` clause.

> [!TIP]
> Remember that basic MySQL statement.
> 
> `SELECT <fieldNameToShow> FROM <tableName> WHERE <condition1> GROUP BY <fieldName2> HAVING <condition2>`

> [!TIP]
> Filter returned value of `FROM` with `WHERE` v.s. filter returned value of `GROUP BY` with `HAVING`.

### view
views are reflection of a table or returned value of subquery.

#### `CREATE VIEW`
See [`CREATE VIEW` MySQL official docs](https://dev.mysql.com/doc/refman/8.0/en/create-view.html)

#### `DROP VIEW`
See [`DROP VIEW` MySQL official docs](https://dev.mysql.com/doc/refman/8.0/en/drop-view.html)
