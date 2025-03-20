# SQL
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
