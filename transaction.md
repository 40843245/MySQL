# MySQL
## transaction
### glossary transaction in MySQL
See [glossary transaction in MySQL (MySQL official docs)](https://dev.mysql.com/doc/refman/8.4/en/glossary.html#glos_transaction)

### transaction type
See [SQL Commands | DDL, DQL, DML, DCL and TCL Commands](https://www.geeksforgeeks.org/sql-ddl-dql-dml-dcl-tcl-commands/)
#### DML transaction (Data Manipulation Language transaction)
#### DDL transaction (Data Definition Language transaction)
#### DCL transaction (Data Control Language transaction)
#### TCL (Transaction Control Language)

### conflicts between many transactions
See 
+ [資料庫 Isolation Levels](https://totoroliu.medium.com/%E8%B3%87%E6%96%99%E5%BA%AB-isolation-levels-c587d3103ba4)
  
#### dirty read
Case in one transaction is writting, another transaction is reading.

![image](https://github.com/user-attachments/assets/2d40bc63-108b-4f25-bf27-c87c6851f2c8)

![image](https://github.com/user-attachments/assets/83c134fe-94c8-486a-be22-19201dbae06b)

### lost update
Case in one transaction is writting, another transaction is writting.

![image](https://github.com/user-attachments/assets/b280e73a-ae7d-4d34-b251-0984714f0878)

![image](https://github.com/user-attachments/assets/3d7fa25c-42a9-4f18-8251-32e4532e708a)

#### non-repeatable read (read skew)
Case in one transaction is writting, another transaction is reading

![image](https://github.com/user-attachments/assets/2a97a102-56f6-44db-a008-46b78c6907a2)

### phantom

![image](https://github.com/user-attachments/assets/8648ea86-1d53-48b5-b29e-d9afee85ee82)

### write skew

![image](https://github.com/user-attachments/assets/f8c04f4d-eaaf-4ff4-8eb6-b122b7dfa3b4)


### solving conflicts between many transactions
See 
+ [資料庫 Isolation Levels](https://totoroliu.medium.com/%E8%B3%87%E6%96%99%E5%BA%AB-isolation-levels-c587d3103ba4)
+ [交易隔離等級 (ODBC) (Microsoft Official docs)](https://learn.microsoft.com/zh-tw/sql/odbc/reference/develop-app/transaction-isolation-levels?view=sql-server-ver16)
+ [isolation level official docs](https://dev.mysql.com/doc/refman/8.4/en/glossary.html#glos_isolation_level)

![image](https://github.com/user-attachments/assets/1c71493f-82c7-4f21-b645-7d62d050d962)

![image](https://github.com/user-attachments/assets/cfc07995-2c32-4a6c-8528-970699f895fc)


### Locking in MySQL

![image](https://github.com/user-attachments/assets/6acf569d-2dbf-4e4f-8ba4-d75f926d682f)  
