# MySQL
## operation about MySQL setting
### automatically commit 
#### `AUTOCOMMIT`

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
### disable safe mode
#### `SET SQL_SAFE_UPDATES=0;`
To disable safe mode (temporarily), executing this MySQL statement.

```
SET SQL_SAFE_UPDATES=0;
```
#### preference setting
To permanently disable safe update mode in MySQL Workbench 8.0, follow these steps.

1. Go to Edit --> Preferences.

2. Click "SQL Editor" tab and uncheck "Safe Updates" (rejects UPDATEs and DELETEs with no restrictions) check box.

3. Query --> Reconnect to Server.

### via
via Rahul Sharma's answer and pankaj's answer on this article.

[Error Code: 1175. You are using safe update mode and you tried to update a table without a WHERE that uses a KEY column](https://stackoverflow.com/questions/30878073/error-code-1175-you-are-using-safe-update-mode-and-you-tried-to-update-a-table)
5. 
