# DataBase Normalization
 Database normalization is a process used to organize a database into tables and columns.  The main idea with this is that a table should be about a specific topic and only supporting topics included.

## Reasons for Database Normalization
 There are three main reasons to normalize a database.
 <br>

 * The first is to minimize duplicate data.
 <br>
 
 * The second is to minimize or avoid data modification issues.
 <br>

 * The third is to simplify queries. 

# Definition of Normalization
 There are three common forms of normalization: 1st, 2nd, and 3rd normal form. There are several additional forms, such as BCNF, but I consider those advanced, and not too necessary to learn in the beginning. The forms are progressive, meaning that to qualify for 3rd normal form, a table must first satisfy the rules for 2nd normal form, and 2nd normal form must adhere to those for 1st normal form. Before we discuss the various forms and rules in details, let’s summarize the various forms:

 * First Normal Form – The information is stored in a relational table and each column contains atomic values, and there are not repeating groups of columns.
 <br>

 * Second Normal Form – The table is in first normal form and all the columns depend on the table’s primary key.
 <br>
 
 * Third Normal Form – The table is in second normal form and all of its columns are not transitively dependent on the primary key.