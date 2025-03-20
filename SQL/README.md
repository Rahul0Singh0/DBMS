![image](https://github.com/user-attachments/assets/a75f8e4a-bfb4-490f-9646-70412ebb834e)# SQL
* SQL is the Structured Query Language.
* It provides standard to RDBMS for accessing and manipulating in relational database.
It helps in:
1. Storing data
2. Retrieving data
3. Updating data
4. Deleting data

### Why SQL?
* Used in almost every database system
* Simple and easy to learn
* Manages large amounts of data efficiently

### Here common SQL databases or RDBMS
1. MySQL – Open-source and widely used
2. PostgreSQL – Advanced open-source database
3. SQL Server – Developed by Microsoft
4. SQLite – Lightweight database, used in mobile apps
5. Oracle Database – Used in enterprise applications

### Note: Using MySQL to learn SQL

## SQL Commands
SQL commands are instructions used to communicate with a database to perform various operations such as creating, reading, updating, and deleting data. These commands are categorized based on their functionality into several types:
### Types
* Data Definition Language (DDL)
* Data Manipulation Language (DML)
* Data Control Language (DCL)
* Transaction Control Language (TCL)
* Data Query Language (DQL)

## Data Definition Language (DDL)
DDL commands are used to define and manage database schema and structure.
### CREATE command
* Creates new database.
* Creates new database objects such as tables, views, and indexes.
* NOTE: In SQL, a view is a virtual table based on the result-set of an SQL statement.
* NOTE: Indexes are used to retrieve data from the database more quickly than otherwise. The users cannot see the indexes, they are just used to speed up searches/queries.
``` SQL
-- case insensitive
CREATE DATABASE EXAMPLE;
USE EXAMPLE;
CREATE TABLE employees (
    id INT PRIMARY KEY,
    name VARCHAR(100),
    position VARCHAR(50),
    salary DECIMAL(10, 2)
);
```
![image](https://github.com/user-attachments/assets/91d766cd-51cc-4df9-8afd-22bc38dfa9aa)


### DROP Command
Deletes existing database objects.
``` SQL
DROP TABLE employees;
```

### ALTER Command
Modifies existing database objects.
``` SQL
ALTER TABLE employees
ADD COLUMN department VARCHAR(50);
```

![image](https://github.com/user-attachments/assets/00b54d96-7e3e-40bf-bae6-f98fe30bde58)

### TRUNCATE Command
Removes all records from a table but retains its structure.
``` SQL
TRUNCATE TABLE employees;
```

## Data Manipulation Language (DML)
DML commands manage data within schema objects.

### INSERT Command
Adds new rows to a table.
``` SQL
INSERT INTO employees (id, name, position, salary)
VALUES (1, 'John Doe', 'Manager', 60000.00);
```
![image](https://github.com/user-attachments/assets/8d137c97-dc57-4791-b4de-57662e3e8591)

### UPDATE Command
Modifies existing rows in a table.
``` SQL
UPDATE employees
SET salary = 65000.00
WHERE id = 1;
```
![image](https://github.com/user-attachments/assets/ab20f4cf-d3f8-46c3-870c-0ad9a117fe5b)

### DELETE Command
Removes existing rows from a table.
``` SQL
DELETE FROM employees
WHERE id = 1;
```

### SELECT Command
Retrieves data from one or more tables.
``` SQL
SELECT id, name, position, salary
FROM employees;
```
![image](https://github.com/user-attachments/assets/93be02c5-c355-4600-bffd-6074c80fbf59)

## Data Control Language (DCL)
DCL commands manage access to data within the database.
### GRANT
Gives a user access privileges to the database.
``` SQL
GRANT SELECT, INSERT, UPDATE ON employees TO user_name;
```

### REVOKE
Removes access privileges from a user.
``` SQL
REVOKE SELECT, INSERT, UPDATE ON employees FROM user_name;
```

## Transaction Control Language (TCL)
TCL commands manage the transactions within a database.

### COMMIT
Saves all changes made in the current transaction.
``` SQL
COMMIT;
```

### ROLLBACK
Undoes changes made in the current transaction.
``` SQL
ROLLBACK;
```
Note: A transaction can't be rolled back after a COMMIT TRANSACTION statement is executed

### SAVEPOINT
Sets a point within a transaction to which you can later roll back.
``` SQL
SAVEPOINT savepoint_name;
```

## Data Query Language (DQL)
DQL is used to retrieve data from a database.
``` SQL
SELECT
SELECT column1, column2, ...
FROM table_name;
```
