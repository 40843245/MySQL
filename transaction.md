# MySQL
## transaction
See [SQL Commands | DDL, DQL, DML, DCL and TCL Commands](https://www.geeksforgeeks.org/sql-ddl-dql-dml-dcl-tcl-commands/)
### DML transaction (Data Manipulation Language transaction)
### DDL transaction (Data Definition Language transaction)
### DCL transaction (Data Control Language transaction)
### TCL (Transaction Control Language)

### conflicts between many transactions
#### dirty read
Case in one transaction is writting, another transaction is reading.

![image](https://github.com/user-attachments/assets/2d40bc63-108b-4f25-bf27-c87c6851f2c8)

### lost update
Case in one transaction is writting, another transaction is writting.

![image](https://github.com/user-attachments/assets/b280e73a-ae7d-4d34-b251-0984714f0878)

### solving conflicts between many transactions
See 
+ [資料庫 Isolation Levels](https://totoroliu.medium.com/%E8%B3%87%E6%96%99%E5%BA%AB-isolation-levels-c587d3103ba4)
+ [交易隔離等級 (ODBC) (Microsoft Official docs)](https://learn.microsoft.com/zh-tw/sql/odbc/reference/develop-app/transaction-isolation-levels?view=sql-server-ver16)

![image](https://github.com/user-attachments/assets/1c71493f-82c7-4f21-b645-7d62d050d962)
