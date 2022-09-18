# Introduction to SQL

SOURCE: [SQLBolt Tutorials](https://sqlbolt.com/)

- A query is a statement which declares what data we are looking for, where to find it in the database, and how to transform it before it is returned.
- SQL databases present as a table, where the rows are a certain instance of the entity and the columns are properties
- Use an '*' ti retrieve all the columns of data when doing a seach
- Add a 'where' clause in the query to filter through millions of rows
- Useful operators for numerical data:

![Useful numeric operators](/reading-notes/img/sql-search-keywords.png)

- Useful operators for text data:

![Useful text operators](/reading-notes/img/sql-text-operators.png)

- SQL provides a convenient way to discard rows that have a duplicate column value by using the DISTINCT keyword
- SQL provides a way to sort your results by a given column in ascending or descending order using the ORDER BY clause
- Other clauses include: The LIMIT will reduce the number of rows to return, and the optional OFFSET will specify where to begin counting the number rows from
- entity data in the real world is often broken down into pieces and stored across multiple orthogonal tables using a process known as normalization
- Tables that share information about a single entity need to have a primary key that identifies that entity uniquely across the database -- use the JOIN clause

![Using INNER JOIN for a search](/reading-notes/img/search-with-inner-join.png)

- In SQL, the database schema is what describes the structure of each table, and the datatypes that each column of the table can contain

- When inserting data into a database, we need to use an INSERT statement, which declares which table to write into, the columns of data that we are filling, and one or more rows of data to insert

- To update rows:

![Update rows statement](/reading-notes/img/update-statement-sql.png)

- use a DELETE statement to delete rows, which describes the table to act on, and the rows of the table to delete through the WHERE clause
- you can create a new database table using the CREATE TABLE statement

- Table data types:

![Table data types](/reading-notes/img/sql-table-date-types.png)

- use the ALTER TABLE statement to add, remove, or modify columns and table constraints
- To remove an entire table (including it's data and metadata) use the DROP TABLE statement, which differs from the DELETE statement in that it also removes the table schema from the database entirely

- Exercise 1-6 & 13-18 completed:

![SQL Exercise One](/reading-notes/img/sql-one.png)
![SQL Exercise Two](/reading-notes/img/sql-two.png)
![SQL Exercise Three](/reading-notes/img/sql-three.png)
![SQL Exercise Four](/reading-notes/img/sql-four.png)
![SQL Exercise Five](/reading-notes/img/sql-five.png)
![SQL Exercise Six](/reading-notes/img/sql-six.png)
![SQL Exercise Thirteen](/reading-notes/img/sql-thirteen.png)
![SQL Exercise Fourteen](/reading-notes/img/sql-fourteen.png)
![SQL Exercise Fifteen](/reading-notes/img/sql-fifteen.png)
![SQL Exercise Sixteen](/reading-notes/img/sql-sixteen.png)
![SQL Exercise Seventeen](/reading-notes/img/sql-seventeen.png)
![SQL Exercise Eighteen](/reading-notes/img/sql-eighteen.png)

[Return home](https://khofstetter94.github.io/reading-notes/)
