# Data Modeling

[nosql vs sql](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

- What type of database is the best fit for the complex query intensive environment?
  - SQL databases are good fit for the complex query intensive environment whereas NoSQL databases are not good fit for complex queries. On a high-level, NoSQL don’t have standard interfaces to perform complex queries, and the queries themselves in NoSQL are not as powerful as SQL query language.
- What type of database is the best fit for hierarchical data storage?
  - SQL databases are not best fit for hierarchical data storage. But, NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data. NoSQL database are highly preferred for large data set (i.e for big data). Hbase is an example for this purpose.
- Describe the differences in scalability between a SQl and NoSQL database as though you were speaking to a non-technical friend.
  - SQL databases are vertically scalable. You can manage increasing load by increasing the CPU, RAM, SSD, etc, on a single server. On the other hand, NoSQL databases are horizontally scalable. You can just add few more servers easily in your NoSQL database infrastructure to handle the large traffic.

[sql modeling techniques](https://www.essentialsql.com/get-ready-to-learn-sql-7-simplified-data-modeling/)

- Among data tables, what is a one-to-many relationship and how do we “relate” them?
  - We connect lines between tables to show relationships.  In some cases an entry in one table can be related to more than one entry in another.  This is called a one-to-many relationship.  For example, there are many animals in one zoo.
- Prior to designing your relational database, it might be useful to ___a___ of the database tables and their relationships.
  - Create a diagram
- Explain the difference between a primary and foreign key.
  - The Primary Keys - Remember the primary keys uniquely identify each row in a table.  A table typically has one primary key, but can have more.  When the key has more than one column, it is called a compound key.
  - Foreign Key – This is a column or set of columns which match a primary key in another table.

[sql vs nosql](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

- How do we treat keywords and parameters differently in SQL syntax?
  - Keywords are used in a database query to help identify tables and columns - such keywords include SELECT, BETWEEN, NOT LIKE, etc. Parameters are used in a query to the database to form the request for specific data.
- Define normalization within the context of schemas and data.
  - Gets rid of redundancy and duplicates in order to enhance integrity and organization.
- Explain the difference between one-to-one, one-to-many, and many-to-many relationships to a non-technical recruiter.
  - One-to-one: One record in one table has a relation to one record in another table
  - One-to-many: One record in one table has a relation to many records in another table
  - Many-to-many: Many records in one table have relations to many records in another table

## Things I want to know more about

- The many ways to traverse a SQL database.

[Return home](https://khofstetter94.github.io/reading-notes/)
