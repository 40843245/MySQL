# MySQL
## operation about MySQL setting
### `AUTOCOMMIT`

> [!IMPORTANT]
> If `AUTOCOMMIT` = 1, it refers automatically commit by MySQL.
>
> If `AUTOCOMMIT` = 1, it refers that it has to finish commission by user.
>
> In this case, user has a chance to rollback (similar to the word regret), one has to execute `COMMIT` to finish the transaction.

To set the status of `AUTOCOMMIT`, use `SET AUTOCOMMIT`.

```
SET @@AUTOCOMMIT = 1; # Enable auto commission mode.
```

```
SET @@AUTOCOMMIT = 0; # Disable auto commission mode.
```
