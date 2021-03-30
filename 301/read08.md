# SQL

### What is SQL?

 Structured Query Language, is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database. And due to its simplicity, SQL databases provide safe and scalable storage for millions of websites and mobile applications.

### Relational databases
Before learning the SQL syntax, it's important to have a model for what a relational database actually is. A relational database represents a collection of related (two-dimensional) tables. Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns (the attributes or properties of the table) and any number of rows of data.

### SELECT
 TO start selecting data from the SQL table:
 <br>

 `SELECT column,another_column FROM tableName;`

 <br>
 <br>
 In order to filter certain results from being returned, we need to use a WHERE clause in the query. The clause is applied to each row of data by checking specific column values to determine whether it should be included in the results or not.
 <br>

 `SELECT column, another_column, … FROM mytable WHERE condition AND/OR another_condition AND/OR …;`
 <br>
 <br>

 ### ORDER BY
 `SELECT column, another_column, … FROM mytable WHERE condition(s) ORDER BY column ASC/DESC;`
