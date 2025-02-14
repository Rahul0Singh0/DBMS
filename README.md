# Introduction to DBMS
### Data
Data is referred to as the collection of raw facts or figures that can be processed to derive meaning or knowledge. It is a collection of information gathered by observations, measurements, research, or analysis. In simpler terms, data is any fact that can be stored, e.g., "EXY", "12", etc.

### Information
* Data when processed becomes Information. 
* Information is the knowledge obtained from investigating, studying, or instructing data.
<b>For Example:</b> Consider the string “orange”. Here, it could mean a color or a fruit. This term “orange” is data. However, if we say “color orange” or “fruit orange”, it becomes information.

## Database
A database is a structured collection of interrelated data organized in a way that enables efficient storage, retrieval, and manipulation of information. Key characteristics of databases include:
* It is a collection of interrelated data.
* It can be stored in the form of tables.
* It can be of any size.

<b>Example of database:</b>
![17395221110214575176719766398525](https://github.com/user-attachments/assets/8a1fd473-7309-4911-abe0-caa5572f27aa)
For example, in a multimedia database, the image table would contain information about images like pixels, length, and width.

Similarly, a college database would have tables like professor and student tables that are related to the timetable for class schedules.

## File System
A file system is a structure that an operating system uses to manage and organize files on a storage device, such as a hard drive or USB flash drive. It defines how data is organized, accessed, and stored on the storage device. The file system acts as an interface between the user and the data.

### Disadvantages of the File System
1. Data Redundancy: Imagine a company using separate spreadsheets for sales, customer contacts, and inventory. If a customer buys a product, their information might be entered in all three spreadsheets, causing duplication.
2. Poor Memory Utilization: Due to storing the same information like customer names and phone numbers in multiple spreadsheets, memory resources are poorly utilized.
3. Data Inconsistency: If a customer's address is updated in the customer contacts spreadsheet but remains unchanged in the sales spreadsheet, it causes data inconsistency.
4. Data Security: File systems do not ensure controlled access to sensitive data. In DBMS, it is possible to limit access to specific data, which protects against unauthorized access.

## Types of database
Mainly two types of database - 
1. Relational Database (Sql)
   It will store the data in tabular form.
   Organized into tables with rows and columns.
   Use SQL to manage data.
   Support ACID (atomicity, consistency, isolation, and durability).
   Ensure data reliability and consistency.
   Good for applications where data consistency is critical.
3. NoSql (Not only Sql)
   NoSQL databases are more flexible and can store data in any structure.
   Can store structured, semi-structured, or unstructured data.
   Handle large data volumes at high speed
   Good for storing large data volumes.

## DBMS and its Applications
A DBMS is a software application that acts as an interface between the data and the end user, allowing users to efficiently store, manage, retrieve, and manipulate large volumes of structured data.
* Organisation: data is arranged into tables in DBMSs, each having a unique collection of rows (like individual books) and columns (like book characteristics).
* Search and Retrieval: users can perform queries to search for specific data using structured query language (SQL) or other interfaces.
* Access Control: access control mechanisms ensure that only authorized users can access certain data, protecting sensitive information.
* Concurrency Control: In a DBMS, concurrency control mechanisms manage multiple users accessing the database simultaneously, preventing data corruption or loss.
* Data Integrity: DBMS ensures data integrity by enforcing rules such as constraints and validations to maintain the accuracy and consistency of the data.

For example: Imagine your college’s library. Your library has thousands of books, and each book contains valuable information. Now, think of your library as a database, and each book as a record in that database.
![17395248332252415117613415333061](https://github.com/user-attachments/assets/1d468954-9333-4cc5-a51a-9a02cf2ac828)
### Applications of DBMS
* Banks
* Schools and Colleges
* E-commerce 
* Enterprise Resource Planning (ERP)

## Need of DBMS
DBMS plays a vital role for businesses, institutions, and organizations to effectively manage and utilize their data. It helps in the following ways:
* Managing Data: DBMS assists in managing operations like inserting, deleting, and manipulating data effectively.
* Ensuring Data Accuracy and Security: DBMS provides access control, ensuring that data is not accessible to unauthorized parties, which guarantees security and data accuracy.
* Supporting Decision-Making: DBMS provides control over how data is handled, which supports essential decision-making for businesses and organizations.
