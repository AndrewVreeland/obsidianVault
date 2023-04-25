[[SQL Lesson 3 Queries with constraints (Pt. 1)]]



Select query for a specific columns

`SELECT column, another_column, … FROM mytable;`

The result of this query will be a two-dimensional set of rows and columns, effectively a copy of the table, but only with the columns that we requested.

If we want to retrieve absolutely all the columns of data from a table, we can then use the asterisk (`*`) shorthand in place of listing all the column names individually.

Select query for all columns

`SELECT * FROM mytable;`

This query, in particular, is really useful because it's a simple way to inspect a table by dumping all the data at once.




