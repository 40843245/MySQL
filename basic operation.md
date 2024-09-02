# MySQL
## basic operation
### database
#### `CREATE DATABASE` clause
To create a database, use `CREATE DATABASE` clause.

```
CREATE DATABASE <databaseName>;
```

See[`CREATE DATABASE` MySQL official docs](https://dev.mysql.com/doc/refman/8.4/en/creating-database.html)

#### `USE DATABASE` clause
To use the database as current database, use `USE` clause.

```
USE <databaseName>;
```

See[`CREATE DATABASE` MySQL official docs](https://dev.mysql.com/doc/refman/8.4/en/creating-database.html)

#### `DATABASE()` function.
To get current database, use `DATABASE()` function.

```
SELECT DATABASE();
```

or 

```
SELECT DATABASE() FROM DUAL;
```

Thanks to cwallenpoole's answer at [stackoverflow](https://stackoverflow.com/questions/8096550/how-to-determine-which-database-is-selected).
### table
#### `CREATE TABLE` clause
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

#### `SELECT` clause
The `SELECT` clause to select and display a variable or a table.

See [`SELECT` MySQL official docs](https://dev.mysql.com/doc/refman/8.0/en/select.html)

#### `INSERT` clause
To insert into data as rows in table, use `INSERT INTO` clause.

See [`INSERT` MySQL official docs](https://dev.mysql.com/doc/refman/8.0/en/insert.html)

