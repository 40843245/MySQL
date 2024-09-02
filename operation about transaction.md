# MySQL
## operation about transaction
### `TRANSACTION`
To begin a transaction, use

```
START TRANSCATION
```

or

```
BEGIN
```

> [!NOTE]
> However, the `BEGIN` clause can be used in other case. Thus, I ***DON'T*** recommend to use it.

### `ROLLBACK`
To rollback to savepoint `<savepoint1>`, canceling the change after savepoint `<savepoint1>`.

`ROLLABCK TO <savepoint1>;`

To rollback to the whole transaction, canceling the whole change. 

`ROLLABCK;`

### `SAVEPOINT`
To create a savepoint, use `SAVEPOINT` clause.

```
SAVEPOINT <savepoint1>;
```

### `COMMIT`
To complete the transaction, use `COMMIT` (when `AUTOCOMMIT` mode is disabled)

```
COMMIT
```

See [`COMMIT` MySQL official docs](https://dev.mysql.com/doc/refman/8.4/en/commit.html)

### `RELEASE`
To free up something, use `RELEASE` clause.

For example, to free up the savepoint, use `RELEASE SAVEPOINT` clause.

It will free up the savepoint <savepoint1>.
```
RELEASE SAVEPOINT <savepoint1>;
```
