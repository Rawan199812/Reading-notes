
## Database normalization 

**Database normalization is a process used to organize a database into tables and columns. The main idea with this is that a table should be about a specific topic and only supporting topics included.**

***By limiting a table to one purpose you reduce the number of duplicate data contained within your database. This eliminates some issues stemming from database modifications.***

- There are three main reasons to normalize a database. The first is to minimize duplicate data, the second is to minimize or avoid data modification issues, and the third is to simplify queries.

- Issues that come up from NOT using Normilization are increases storage and decreases performance and becomes difficult to maintain storage.

- SPREAD OUT THE DATA ACROSS DIFFERENT TABLES OF LIKE MINDED DATA! OTHERWISE WE GET INCONSISTENT DATA!

Sorting will become very difficult

**First Normal Form – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.**
**Second Normal Form – The table is in first normal form and all the columns depend on the table’s primary key.**
**Third Normal Form – the table is in second normal form and all of its columns are not transitively dependent on the primary key**
