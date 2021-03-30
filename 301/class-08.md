## SQL
**SQL is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database. And due to its simplicity, SQL databases provide safe and scalable storage for millions of websites and mobile applications.**

***There are many popular SQL databases:***
SQLite
MySQL
Postgres
Oracle
relational database actually is. A relational database represents a collection of related tables. Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns and any number of rows of data.
To retrieve data from a SQL database, we need to write SELECT statements, which are often colloquially refered to as queries. A query in itself is just a statement which declares what data we are looking for, where to find it in the database for example "
Select query for a specific columns
SELECT column, another_column, …
FROM mytable;
Or for example :
Select query for all columns
SELECT *
FROM mytable;
Some SQL operators:
=, !=, < <=, >, >= Standard numerical operators
BETWEEN … AND … Number is within range of two values (inclusive)
IN (…) Number exists in a list
NOT IN (…) Number does not exist in a list
- SQL provides a convenient way to discard rows that have a duplicate column value by using the DISTINCT keyword for **example :**
Select query with unique results
SELECT DISTINCT column, another_column, …
FROM mytable
WHERE condition(s);
- When inserting data into a database, we need to use an INSERT statement, which declares which table to write into, the columns of data that we are filling, and one or more rows of data to insert.
When you need to delete data from a table in the database, you can use a DELETE statement,
When you have new entities and relationships to store in your database, you can create a new database table using the CREATE TABLE statement.

- SQL provides a way for you to update your corresponding tables and database schemas by using the ALTER TABLE statement to add, remove, or modify columns and table constraints.
- you can use the DROP TABLE statement, which differs from the DELETE statement in that it also removes the table schema from the database entirely.