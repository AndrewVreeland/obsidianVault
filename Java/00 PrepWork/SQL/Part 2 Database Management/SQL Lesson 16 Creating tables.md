
[[SQL Lesson 17 Altering tables]]


When you have new entities and relationships to store in your database, you can create a new database table using the `CREATE TABLE` statement.

Create table statement w/ optional table constraint and default value

`CREATE TABLE IF NOT EXISTS mytable ( column _DataType_ _TableConstraint_ DEFAULT _default_value_, another_column _DataType_ _TableConstraint_ DEFAULT _default_value_, … );`

The structure of the new table is defined by its _table schema_, which defines a series of columns. Each column has a name, the type of data allowed in that column, an _optional_ table constraint on values being inserted, and an optional default value.

If there already exists a table with the same name, the SQL implementation will usually throw an error, so to suppress the error and skip creating a table if one exists, you can use the `IF NOT EXISTS` clause.

# Table data types

Different databases support different data types, but the common types support numeric, string, and other miscellaneous things like dates, booleans, or even binary data. Here are some examples that you might use in real code.


![[Screenshot 2023-04-15 233527.png]]
[MYSQL](http://dev.mysql.com/doc/refman/5.6/en/data-types.html) [Postgres](http://www.postgresql.org/docs/9.4/static/datatype.html) [SQLite](https://www.sqlite.org/datatype3.html) [Microsoft SQL Server](https://msdn.microsoft.com/en-us/library/ms187752.aspx)

## Table constraints

We aren't going to dive too deep into table constraints in this lesson, but each column can have additional table constraints on it which limit what values can be inserted into that column. This is not a comprehensive list, but will show a few common constraints that you might find useful.

![[Screenshot 2023-04-15 233836.png]]

## An example

Here's an example schema for the _Movies_ table that we've been using in the lessons up to now.

Movies table schema

`CREATE TABLE movies ( 
`id INTEGER PRIMARY KEY, 
`title TEXT, 
`director TEXT,
`year INTEGER, 
`length_minutes INTEGER );`