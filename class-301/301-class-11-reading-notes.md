# Mongo and Mongoose

[nosql vs sql](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

[sql vs nosql (Video)](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

- **Fill in the chart below with five differences between SQL and NoSQL databases:**

|SQL        |NoSQL|
|-----------|-----|
| Data uses schemas |  schema-less   |
|  Relations  |   No (or very few) relations  |
|   Data is distributed across multiple tables |  Data is merged/nested in a few collections   |
|   Horizontal scaling is hard/impossible, and vertical is possible  |   both horizontal and vertical scaling is possible   |
|  Limitations for lots of (thousands) read & write queries per second  |  Great performance for mass(simple) read & write requests   |

- **What kind of data is a good fit for an SQL database?** - SQL databases are good fit for the complex query intensive environment
- **Give a real world example.** - Relatively flat data such as unnested or primitive types like strings and numbers. Example would be a restaurant menu.
- **What kind of data is a good fit a NoSQL database?** - NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data.
- **Give a real world example.** - Nested data or more complex data like arrays, for example an address book.
- **Which type of database is best for hierarchical data storage?** - NoSQL
- **Which type of database is best for scalability?** - SQL is best for vertically scaled and NoSQL is best for horizontally scaled.

- **What does SQL stand for?** - Structured Query Language
- **What is a relational database?** - This means we have a database which works with certain assumptions or in a certain way, and it supports the structured query language.
- **What type of structure does a relational database work with?** - tables
- **What is a ‘schema’?** - a representation of a plan. It is defined as so-called fields in a table. All records have to follow the scheme of the table.
- **What is a NoSQL database?** - involves a database with collections and documents what do not have to use the same schema. There are also no relations.
- **How does it work?** - You put all the information in one place (collections) - and every collection has the information it needs without having to have relation merging. It has super fast querying power.
- **What is inside of a Mongo database?** -
- **Which is more flexible - SQL or MongoDB? and why.** - MongoDB is more flexible due to not having to adhere to a strict schema and not having relations.
- **What is the disadvantage of a NoSQL database?** - being schema-less can make it more unreliable for some collections to have a certain field. Have little to no relations can be a disadvantage if you have a lot of write requests that affect multiple collections.

## Things I want to know more about

- Examples of SQL and NoSQL. Demonstrations of how some kind of data would work best for one and not the other.

[Return home](https://khofstetter94.github.io/reading-notes/)
