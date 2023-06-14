[Spring guide: Accessing Data with JPA](https://spring.io/guides/gs/accessing-data-jpa/)

1.  How are query methods defined when using Spring Data JPA?
	1. define query methods by declaring their method signature
2.  Which dependencies will you need in order to complete the Spring guide?
	1. **Spring Data JPA** and then **H2 Database**.
3.  What annotations are used to specify an auto generated identification number for an Entity?
	1. @GeneratedValue and @Id
	2. The `Customer` object’s `id` property is annotated with `@Id` so that JPA recognizes it as the object’s ID. The `id` property is also annotated with `@GeneratedValue` to indicate that the ID should be generated automatically.

[Baeldung: Comparing repositories](https://www.baeldung.com/spring-data-repositories) (we’ll be using JpaRepository)

1.  Which of the Spring Data Repositories covered in the readings has the most methods available to it?
	1. **_JpaRepository_**
2.  Name a downside of a Spring Data Repository.
	1.   we couple our code to the library and to its specific abstractions, such as `Page` or `Pageable`; that's of course not unique to this library – but we do have to be careful not to expose these internal implementation details
2.  by extending e.g. _CrudRepository_, we expose a complete set of persistence method at once. This is probably fine in most circumstances as well but we might run into situations where we'd like to gain more fine-grained control over the methods exposed, e.g. to create a _ReadOnlyRepository_ that doesn't include the _save(…)_ and _delete(…)_ methods of _CrudRepository_
3.  How would you define an operation to find a student based on their name in a repo named StudentRepository which extends JpaRepository?
	1. public interface StudentRepository extends JpaRepository<Student, Long> { List<Student> findByName(String name); }
			1. student class would need to extend serializable. 