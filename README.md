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

## Data Abstraction
Database systems are built with complex ways of organizing data. To make it easier for people to use the database, the creators hide the complicated details that users don't need to worry about. This hiding of unnecessary complexities from users is called data abstraction.

For example: A user will not be concerned about indexing, memory storage locations, or what data structures are used behind the scenes. The user can directly interact with the database without needing to understand these underlying complexities.

### Levels of Abstraction
There are three levels of data abstraction:
![17395271813233575711500381173776](https://github.com/user-attachments/assets/396a28c2-2b3e-4c87-b298-d6fe4e255ce8)

#### Physical Level:
This is the lowest level of data abstraction. It describes how data is stored in a database, providing details about complex data structures.

For example: Think of a library storing books. The physical level involves how the books are physically stored on shelves, the materials used to make the shelves, and how the shelves are arranged within the library space.

#### Logical Level:
This is the middle level of the 3-level data abstraction architecture. It describes what data is stored in the database and how it is structured.

For example: Consider a library's catalogue system. At the logical level, it’s like looking at how books are categorised and indexed for easy retrieval. This includes details like the indexing methods used and how books are classified by subject, author, and title. It helps visitors search and find books based on their interests.

#### View Level:
This is the highest level of data abstraction. It describes the interaction between users and the database system, focusing on what users can see and access.

For example: In a library, different visitors may have different levels of access. At the view level, it's like determining who can borrow specific types of books or access restricted sections based on their role or membership level.

## Data Architecture
A schema is a logical container or structure that organises and defines the structure of a database.

It defines how data is organised, what data types are used, what constraints are applied, and the relationships between different pieces of data. A schema acts as a blueprint for the database, ensuring data integrity, consistency, and efficient data retrieval.

![17395275118565466262027821988647](https://github.com/user-attachments/assets/489ca191-9e95-493c-a0c4-aaf66bac1f82)

### Types of Schema
#### Physical Schema: 
A physical schema defines how data is stored on the underlying hardware, including details such as storage format, file organisation, indexing methods, and data placement.
#### Logical Schema
## Logical Schema
A logical schema defines the database’s structure from a logical or conceptual perspective, without considering how the data is physically stored.
![17395277344381701414972393489261](https://github.com/user-attachments/assets/2e196fff-c584-4e9d-87c5-2450aac7968a)

### Conceptual Schema: 
The conceptual schema represents the overall view of the entire database. It defines the high-level structure and relationships between all data elements.

For example: Consider a university database with entities such as Student, Course, and Department. 
Relationships among them are: 
* Students can enrol in multiple Courses.
* Each Course can be taken by multiple students.
* Each Course is offered by one Department, but a Department can offer multiple courses.

Note: The focus is on what the data represents (students, courses, departments) and how these entities are interrelated through relationships like enrollment and offerings.

### External/View Schema: 
An external schema defines the user-specific views of the database. It focuses on the portions of the database that are relevant to specific user roles or applications.

For example: In a university database, for a Student's Portal, the view will have StudentProfile. This view provides a student with access to their data and their course enrollments, but not to other students' information or course details like credits or department.

### Instance
The term "instance" in this context denotes the current values of these variables at a particular moment in time for that database.
![17395289223113236865712337908942](https://github.com/user-attachments/assets/7ea3e748-d7e6-4122-84d8-8f05a96f4dc8)

## 3-Tier DBMS Architecture
3-tier architecture is the most widely used architecture in real-world large and complex web applications like Facebook. This architecture separates the application into three logically distinct layers:

* Presentation Layer - Handles the user interface
* Application Layer - Manages business logic
* Data Layer - Manages data storage and processing

In this architecture, the end user has no idea about the existence of the database beyond the application server. Similarly, the database has no knowledge about any other user beyond the application.

Let us imagine an online shopping scenario. Whenever you go onto a platform like Amazon and perform an operation, such as searching for a product or adding an item to your cart, you interact with the frontend or User Interface (UI) of the application, which is represented by the Presentation Layer.

Any operation performed at the presentation layer gets sent to the next layer, the Application Layer, as a request. Upon receiving the request, the application layer interprets the request, formulates a corresponding database query, and sends it to the Data Layer. The data layer, which stores all the data, receives the query and executes it against the database.

Relevant information, such as product details and user account information, is retrieved, and the results are sent back to the application layer. The application layer processes the data further if necessary (e.g., formatting) and sends the response back to the presentation layer. The presentation layer then presents the results to the user, completing the process.
![17395296487623660268080924641727](https://github.com/user-attachments/assets/ba2c35c9-4d54-4734-b1cd-e8d76b1541e5)

### Advantages of 3-Tier Architecture
1. Scalability: Enhanced scalability due to the distributed deployment of application servers. Each layer can be adjusted without altering other layers.
2. Security: The client does not directly interact with the server, providing an added layer of security.
3. Modularity and Maintainability: Maintenance is simplified due to the separation of responsibilities.
4. Performance: Individual optimisation of presentation or application tiers is possible, leading to better performance.

### Disadvantages of 3-Tier Architecture
1. Increased Complexity: The introduction of an extra middle layer increases the complexity of the system. Communication points are also doubled.
2. Potential Latency Issues and Bottlenecks: The added step of processing increases the possibility of latency and bottlenecks, as problems can arise in any layer at any time.
3. Longer Development Time: Implementing three tiers with different logics and distributed responsibilities results in longer development time.
4. Resource Overhead: Implementing an extra tier causes resource overhead for development, processing, and maintenance of the architecture.

# Data Models
A data model in a DBMS is an abstract way to represent how data is structured and organized within a database. It shows the logical arrangement of data and the connections between different data components. Data models are crucial for understanding and designing databases, linking real-world entities to actual data storage.

For instance, before writing an algorithm for “Making Maggi,” having a flowchart makes it easier to implement the algorithm. Similarly, having a data model helps in understanding the relationships between different components in the database.

## Types of Data Models
### Hierarchical Data Model
This model displays data in a tree structure, where each record has a parent-child relationship. It is mainly used in older database systems.

For example, 
![17395312826213034478396773688164](https://github.com/user-attachments/assets/3334105a-b1ef-42db-8b99-9fd3e172e43d)

### Network Data Model
This model allows records to have multiple parent-child relationships, resembling a graph. It offers more flexibility than the hierarchical model.

For example, the image shows that "Student" has both "Lab" and "School" as parents.
![17395313268211091406306986262682](https://github.com/user-attachments/assets/ad8a5dd1-4165-498f-bf80-16fedca3838d)

### Relational Data Model
The relational model organizes data into tables (known as relations) with rows and columns. It is the most common data model and is based on set theory, using Structured Query Language (SQL) for data manipulation.

Example: A customer database where customers are stored in a table with attributes like name, address, and phone number.

### Entity-Relationship Model (ER Model)
The ER model is used to design relational databases by representing data as entities (objects), attributes (properties of entities), and the relationships connecting these entities.

For example, the entity "Student" has an attribute "S.Name" and a relationship with the entity "Courses."

### Object-Oriented Data Model
This model applies the principles of object-oriented programming to databases. It represents data as objects with attributes and methods, supporting inheritance and encapsulation.

Example: A product in an e-commerce system can be represented as an object with properties like price, description, and methods to calculate discounts.

### NoSQL Data Models
NoSQL databases offer various data models, including:

* Document-oriented (e.g., MongoDB)
* Key-value (e.g., Redis)
* Column-family (e.g., Cassandra)
* Graph (e.g., Neo4j)

These models are designed for scalability and flexibility, particularly when managing large amounts of unstructured or semi-structured data.

## Entity and Its Types
An Entity is something from the real world, like a person, place, event, or idea. Each entity has specific features or traits that describe it.

There are two types of entities:
### Strong Entity
A strong entity is an entity that has its unique identifier (primary key) and is not dependent on any other entity for its existence within the database. Strong entities stand alone and have their own set of attributes. For Example- An entity “person” can exist independently.

### Weak Entity
A weak entity is an entity that doesn't have a primary key of its own. It relies on a related strong entity (known as the "owner" entity) for its identity. The weak entity’s existence is defined by being related to the owner entity. For example- In a company, employees can file for dependents under their name. In this case, the entity, “Dependents” is weak.
![17395316856568313674779667794494](https://github.com/user-attachments/assets/46880b0e-084c-4042-8c17-5777ef4463b1)

From the figure, it can be seen that the “Student” table is a strong entity as it can exist independently. However, the “Course” table has a foreign key of S.ID (as explained here). This makes the “course” entity dependent on the “Student” entity. Hence, the “course” entity is a weak entity.
![17395317913369049110837190535898](https://github.com/user-attachments/assets/686838f6-904b-4867-8508-4e7e1aee1955)

## Extended ER Features
The Extended Entity-Relationship (EER) model is an enhancement of the basic Entity-Relationship (ER) model used in database design. It includes additional features that provide more detail and allow for a more accurate representation of complex real-world scenarios.
