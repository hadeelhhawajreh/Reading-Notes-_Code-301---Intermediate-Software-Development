Readings: SQL

![img](https://miro.medium.com/max/1200/1*Oe7xavCj5qCBzwTbLDbPTg.jpeg)


# SQL is a standard language for storing, manipulating and retrieving data in databases.

Our SQL tutorial will teach you how to use SQL in: MySQL, SQL Server, MS Access, Oracle, Sybase, Informix, Postgres, and other database systems.

``SELECT * FROM table;``
``SELECT * FROM Customers;``

- What is SQL?
  SQL stands for Structured Query Language
  SQL lets you access and manipulate databases
  
  SQL became a standard of the American National Standards Institute (ANSI) in 1986, and of the International Organization for Standardization (ISO) in 1987
  
+ What Can SQL do?

  SQL can execute queries against a database
  SQL can retrieve data from a database
  SQL can insert records in a database
  SQL can update records in a database
  SQL can delete records from a database
  SQL can create new databases
  SQL can create new tables in a database
  SQL can create stored procedures in a database
  SQL can create views in a database
  SQL can set permissions on tables, procedures, and views


![exapmle](https://d2mvzyuse3lwjc.cloudfront.net/doc/en/UserGuide/images/The_SQL_Editor_Dialog_Box/Sqleditor.png?v=84550)

Every table is broken up into smaller entities called fields. The fields in the Customers table consist of CustomerID, CustomerName, ContactName, Address, City, PostalCode and Country. A field is a column in a table that is designed to maintain specific information about every record in the table.

A record, also called a row, is each individual entry that exists in a table. For example, there are 91 records in the above Customers table. A record is a horizontal entity in a table.

A column is a vertical entity in a table that contains all information associated with a specific field in a table





+ Using SQL in Your Web Site
  To build a web site that shows data from a database, you will need:
  An RDBMS database program (i.e. MS Access, SQL Server, MySQL)
  To use a server-side scripting language, like PHP or ASP
  To use SQL to get the data you want
  To use HTML / CSS to style the page
  
 -RDBMS
  RDBMS stands for Relational Database Management System.

  RDBMS is the basis for SQL, and for all modern database systems such as MS SQL Server, IBM DB2, Oracle, MySQL, and Microsoft Access.

  The data in RDBMS is stored in database objects called tables. A table is a collection of related data entries and it consists of columns and rows.
  
  ### SQL keywords are NOT case sensitive: select is the same as SELECT

  
  
  
  *Some of The Most Important SQL Commands*
   **SELECT** - extracts data from a database
   
   **UPDATE**- updates data in a database
   
   **DELETE** - deletes data from a database
   
   **INSERT INTO** - inserts new data into a database
   
   **CREATE DATABASE** - creates a new database
   
   **ALTER DATABASE** - modifies a database
   
   **CREATE TABLE** - creates a new table
   
   **ALTER TABLE** - modifies a table
   
   **DROP TABLE** - deletes a table
   
   **CREATE INDEX** - creates an index (search key)
   
   **DROP INDEX**- deletes an index
   SQL SELECT Statement

   >SELECT column1, column2, ...FROM table_name;
>SELECT * FROM Customers; ---> selects all the columns from the "Customers" table



SQL WHERE Statement

*The WHERE clause is used to filter records.*

>selects all the customers from the country "Mexico", in the "Customers" table

``SELECT * FROM Customers``
``WHERE Country='Mexico';``
``SQL AND, OR and NOT Operators``

*The AND and OR operators are used to filter records based on more than one condition*

>AND Syntax

``SELECT * FROM Customers``
``WHERE Country='Germany' AND City='Berlin';``
>OR 

``SELECT * FROM Customers``
``WHERE Country='Germany' OR Country='Spain';``
>NOT 

``SELECT * FROM Customers``
``WHERE NOT Country='Germany';``
