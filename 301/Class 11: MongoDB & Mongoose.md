# MongoDB and Mongoose

[nosql vs sql](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

## What kind of data is a good fit for an SQL database?

> A good fit for an SQL database is structured data with a well-defined schema. SQL databases are ideal for data that has a fixed and consistent structure, where relationships between different tables are essential for querying and processing the data efficiently. Some examples of data that fit well in an SQL database are:

## Give a real world example.

> Let's consider an e-commerce store as an example. The store's SQL database would have tables for customers, products, orders, and payments. Each of these tables would have predefined columns, such as customer name, address, product ID, product name, price, order date, payment information, etc. The relational nature of SQL databases allows us to link data between tables, enabling queries like finding all orders made by a specific customer or retrieving the products in a particular order.

## What kind of data is a good fit a NoSQL database?

> A good fit for a NoSQL database is semi-structured or unstructured data where the schema can evolve over time or where data does not have well-defined relationships. NoSQL databases are more flexible and can handle large volumes of rapidly changing data. Some examples of data that fit well in a NoSQL database are:

## Give a real world example.

> A social media platform generates vast amounts of unstructured data, including user-generated content, comments, likes, and shares. Since social media data can vary greatly in structure and evolve frequently (e.g., new types of posts or interactions), a NoSQL database, such as MongoDB or Cassandra, would be more suitable for storing and managing this dynamic and diverse data.

## Which type of database is best for hierarchical data storage?

> For hierarchical data storage, a type of database called a Hierarchical Database Management System (Hierarchical DBMS) is most suitable. Hierarchical databases use a tree-like structure to organize data, where each parent node can have multiple child nodes, but each child node has only one parent. This type of database is best suited for data with inherent hierarchical relationships.

> One common example of hierarchical data is a file system on a computer. Directories (folders) can contain files or subdirectories, and those subdirectories can have their own files or subdirectories. This hierarchical structure is effectively managed by a Hierarchical DBMS, making it easy to navigate and access files based on their location in the directory tree.

## Which type of database is best for scalability?

> For scalability, NoSQL databases are generally preferred. NoSQL databases are designed to handle large volumes of data and high levels of read and write operations across distributed systems. They can easily scale horizontally by adding more servers to the database cluster, which allows for seamless expansion and improved performance as the data and traffic grow.

> Real World Example: Web Application with High User Traffic
Consider a web application with millions of users that require real-time data processing, like a social networking site, where users are constantly posting updates, liking posts, and generating a huge amount of data. To handle this high level of scalability, a NoSQL database like Apache Cassandra or Amazon DynamoDB would be a better choice. These databases can distribute data across multiple nodes and ensure efficient handling of concurrent read and write requests, making them highly scalable solutions.

[sql vs nosql](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

## What does SQL stand for?

> SQL stands for "Structured Query Language." It is a domain-specific language used to manage and manipulate relational databases.

## What is a relational database?

A relational database is a type of database management system that organises data into tables with rows and columns, where each row represents a record and each column represents a data attribute. The relationships between different tables are defined through keys, which establish connections between related data.

## What type of structure does a relational database work with?

A relational database works with a tabular structure, where data is organised into tables (relations), and each table contains rows (tuples) and columns (attributes).

## What is a ‘schema’?

A 'schema' in the context of databases refers to the structure or blueprint that defines the organisation of data within a database. It defines the tables, their columns, data types, constraints, and relationships between tables, ensuring data integrity and consistency.

## What is a NoSQL database?

> A NoSQL database (Not Only SQL) is a type of database management system that does not adhere to the traditional tabular structure of relational databases. Instead, it provides a more flexible approach for handling and storing various types of data, including unstructured, semi-structured, and structured data. NoSQL databases are often used for large-scale, distributed, and real-time applications.

## How does it work?

> NoSQL databases work differently depending on the specific type, but in general, they use a variety of data models such as document-oriented, key-value, column-family, or graph databases. These databases are designed to be horizontally scalable and can distribute data across multiple nodes in a cluster to handle high volumes of data and traffic efficiently.

## What is inside of a MongoDB database?

> Inside a MongoDB database, the data is organized into collections, which are analogous to tables in a relational database. Each collection contains JSON-like documents that represent individual records. These documents can have different structures, allowing for more flexible data storage.

## Which is more flexible - SQL or MongoDB? and why.

> MongoDB is more flexible than traditional SQL databases because it is a NoSQL database. It does not enforce a fixed schema, meaning that each document in a collection can have different fields, and new fields can be added at any time without affecting other documents. This schema-less nature allows developers to adapt the data model quickly and easily to changing application requirements.

## What is the disadvantage of a NoSQL database?

> The disadvantage of a NoSQL database, including MongoDB, is the potential for reduced data consistency. Since NoSQL databases often prioritise availability and partition tolerance over consistency (CAP theorem), there might be cases where data reads may not reflect the latest writes immediately (eventual consistency). This trade-off is acceptable for many use cases, but it might not be suitable for applications requiring strong ACID (Atomicity, Consistency, Isolation, Durability) guarantees like financial systems or transaction-intensive applications. Additionally, since NoSQL databases often lack standardised query languages like SQL, querying and reporting can be more challenging for developers who are used to SQL-based querying.

[Mongoose.API](https://mongoosejs.com/docs/api.html#Model)
[React Router](https://reactrouter.com/web/api/BrowserRouter)





