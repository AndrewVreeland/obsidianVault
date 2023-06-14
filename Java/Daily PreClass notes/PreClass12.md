[Many to many relationships](https://www.baeldung.com/hibernate-many-to-many)

1.  Name a few examples of real world ManyToMany relationships.
	 -   A music streaming service where many users can follow many different artists, and each artist can have many different followers.
	  -   A social media platform where users can belong to many different groups, and each group can have many different members.
	  -   A university where many students can enroll in many different courses, and each course can have many different students.
1.  Explain the significance of a join table for ManyToMany relationships.
	1.  The significance of a join table for ManyToMany relationships is that it allows for the association between the two tables without creating redundant data. In a ManyToMany relationship, each record in Table A can be associated with many records in Table B, and each record in Table B can be associated with many records in Table A. Without a join table, this would require duplicating data in one of the tables, which can lead to data inconsistencies and performance issues.
2.  What are the values held within a join table?
	The values held within a join table are typically the primary keys of the two tables being joined. For example, in a ManyToMany relationship between students and courses, the join table might have columns for student_id and course_id. Each row in the join table represents a unique association between a student and a course.
[Security: a humorous overview](http://scholar.harvard.edu/files/mickens/files/thisworldofours.pdf)

1.  According to the author of the article, will you ever be truly secure from ALL possible security threats?
	1. threats will always exsist!