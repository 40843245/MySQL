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
To rollback to savepoint `<savepoint1>`.

`ROLLABCK TO <savepoint1>;`

To rollback to the whole transaction.

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

