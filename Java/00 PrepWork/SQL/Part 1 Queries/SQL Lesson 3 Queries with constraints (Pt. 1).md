
[[SQL Lesson 4 Queries with constraints (Pt. 2)]]
[[SQL Lesson 2 Queries]]
In order to filter certain results from being returned, we need to use a `WHERE` clause in the query. The clause is applied to each row of data by checking specific column values to determine whether it should be included in the results or not.

Select query with constraints

`SELECT column, another_column, … FROM mytable **WHERE _condition_ AND/OR _another_condition_ AND/OR …**;`

More complex clauses can be constructed by joining numerous `AND` or `OR` logical keywords (ie. num_wheels >= 4 AND doors <= 2). And below are some useful operators that you can use for numerical data (ie. integer or floating point):


SQL Example

1. =, !=, < <=, >, >= 
		1. CONDITION: Standard numerical operators      
		2. EXAMPLE:  col_name != 4
2. BETWEEN … AND …
	1. CONDITION: Number is within range of two values (inclusive)
	2. EXAMPLE: col_name BETWEEN 1.5 AND 10.5
3. NOT BETWEEN … AND …
	1. CONDITION: Number is not within range of two values (inclusive)
	2. EXAMPLE: col_name NOT BETWEEN 1 AND 10
4. IN (…)
	1. CONDITION: Number exists in a list
	2. EXAMPLE: col_name IN (2, 4, 6)
5. NOT IN (…)
	1. CONDITION: Number does not exist in a list
	2. EXAMPLE: col_name NOT IN (1, 3, 5)

In addition to making the results more manageable to understand, writing clauses to constrain the set of rows returned also allows the query to run faster due to the reduction in unnecessary data being returned.

Did you know?

As you might have noticed by now, SQL doesn't _require_ you to write the keywords all capitalized, but as a convention, it helps people distinguish SQL keywords from column and tables names, and makes the query easier to read.