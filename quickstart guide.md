# MySQL
## installation
### install free version of MySQL server  
To install free version of MySQL server to your device. Follow these steps.

1. visit [MySQL Downloads](https://dev.mysql.com/downloads/mysql/8.0.html).
2. select the version.
3. select OS.
4. according to your needs and system requirement (such as Windows x64 or Windows x84), check the corresponding item and click `Download` button on the rightmost of the item. It will install an installation exe.
5. Click installation exe. It will open the wizard for installation.
6. Configure the settings in wizard for installation.
7. Click `execute` button.
8. Wait until the download is completed.
9. Add the directory of `mysql.exe` to system environment variable `$PATH`.
10. That's done. 

> [!CAUTION]
> Please remember your password. The password is required when you login the MySQL server.
>
> If you forgot it. It may be cumbersome.
>
> I think the easiest way to solve it is that to reinstall it again (which is tad cumbersome).

### install free version of MySQL workbench
1. visit [MySQL workbench Downloads](https://dev.mysql.com/downloads/workbench/)
2. select OS.
3. according to your needs and system requirement (such as Windows x64 or Windows x84), check the corresponding item and click `Download` button on the rightmost of the item. It will install an installation exe.
4. Click installation exe. It will open the wizard for installation.
5. Configure the settings in wizard for installation.
6. Click `execute` button.
7. Wait until the download is completed.
8. That's done.

## use
To type the MySQL command, either

+

> [!IMPORTANT]
> It does NOT require that the system environment variable `$PATH` contains the directory of `mysql.exe` (which is mentioned step 9 under [`installation` section](#installation)).

  1. open MySQL 9.0 command client.
  2. enter the password to login.

+

> [!IMPORTANT]
> It requires that the system environment variable `$PATH` contains the directory of `mysql.exe` (which is mentioned step 9 under [`installation` section](#installation)).


  1. open DOS.
  2. run these commands.

```
mysql --user=<userName> --password
```

  3. enter the password to login.

