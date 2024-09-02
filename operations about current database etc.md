# MySQL
## operations about current database etc
### database
#### get current database

```
SELECT DATABASE();
```

### table
#### describe table info

```
DESCRIBLE <tableName>;
```

Or in newer version of MySQL, it can be abbreviated as 

```
DESC <tableName>;
```

#### show all tables in current database

```
SHOW DATABASES;
```

#### show all records of given table

```
SELECT * FROM <tableName>;
```

#### create table
Use `CREATE TABLE` clause.

```
CREATE TABLE(
``<field>
  [,<field>]
);
```

#### insert data into table
Use `INSERT INTO` clause.

+ 1th form:
```
INSERT INTO <tableName> (<fieldName1> [, <fieldName2>]) VALUES (<fieldValue1> [, <fieldValue2>]);
```

+ 2th form:

NOTICE that there are NO `VALUE` clause in second form.

```
INSERT INTO <tableName> (<fieldValue1> [, <fieldValue2>]);
```

+ 3th form:
  
```
INSERT INTO <tableName> (<fieldValue>,);
```

#### update one or more records in table

```
UPDATE <tableName> SET <fieldName1> = <newValue1> [, <fieldName2> = <newValue2> ][WHERE <condition>];
```

#### delete one or more records in table

```
DELETE FROM <tableName> [WHERE <condition>];
```

#### drop table
To drop a table, use `DROP TABLE` clause.

```
DROP TABLE <tableName>;
```

### view
Similar to operation for [table](#table).
