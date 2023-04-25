[[SQL Lesson 5 Filtering and sorting Query results]]
[[SQL Lesson 2 Queries]]
SQL Lesson 3: Queries with constraints (Pt. 2)

When writing `WHERE` clauses with columns containing text data, SQL supports a number of useful operators to do things like case-insensitive string comparison and wildcard pattern matching. We show a few common text-data specific operators below:



1. OPERATOR: = 
	1. CONDITION: Case sensitive exact string comparison (_notice the single equals_)
	2. EXAMPLE: col_name = "abc"

2. != or <>
	1. Case sensitive exact string inequality comparison
	2. col_name != "abcd"

3. LIKE
	1. Case insensitive exact string comparison
	2. col_name LIKE "ABC"

4. NOT LIKE
	1. Case insensitive exact string inequality comparison
	2. col_name NOT LIKE "ABCD"

5. %
	1. Used anywhere in a string to match a sequence of zero or more characters (only with LIKE or NOT LIKE)
	2. col_name LIKE "%AT%"  
(matches "AT", "ATTIC", "CAT" or even "BATS")

6. _
	1. Used anywhere in a string to match a single character (only with LIKE or NOT LIKE)
	2. col_name LIKE "AN_"  (matches "AND", but not "AN")

7. IN (…)
	1. String exists in a list
	2. col_name IN ("A", "B", "C")

8. NOT IN (…)
	1. String does not exist in a list
	2. col_name NOT IN ("D", "E", "F")

Did you know?

All strings must be quoted so that the query parser can distinguish words in the string from SQL keywords.

We should note that while most database implementations are quite efficient when using these operators, full-text search is best left to dedicated libraries like [Apache Lucene](http://lucene.apache.org/ "Apache Lucene") or [Sphinx](http://sphinxsearch.com/ "Sphinx Search"). These libraries are designed specifically to do full text search, and as a result are more efficient and can support a wider variety of search features including internationalization and advanced queries.