[Overview: Saving data with Room](https://developer.android.com/training/data-storage/room)

- The Room persistence library is part of Android Jetpack and provides an abstraction layer over SQLite for efficient database access.
- Room offers benefits such as compile-time verification of SQL queries, convenience annotations to minimize boilerplate code, and streamlined database migration paths.
- It is recommended to use Room instead of directly using SQLite APIs.
- To set up Room in your app, you need to add the necessary dependencies to your app's build.gradle file.
- The primary components of Room are the database class, data entities, and data access objects (DAOs).
- The database class serves as the main access point to the app's persisted data and provides instances of the associated DAOs.
- Data entities represent tables in the database and are defined using annotations.
- DAOs define methods for querying, updating, inserting, and deleting data in the database.
- An example implementation of a Room database includes a User data entity and a UserDao DAO.
- The User data entity represents a row in the user table and contains relevant fields.
- The UserDao DAO provides methods like getAll(), loadAllByIds(), findByName(), insertAll(), and delete() to interact with the user table.
- The AppDatabase class holds the database and extends RoomDatabase.
- The AppDatabase class must be annotated with @Database and include an entities array listing the associated data entities.
- Abstract methods in the AppDatabase class return instances of the associated DAO classes.
- It is recommended to follow the singleton design pattern when instantiating an AppDatabase object.
- Usage involves creating an instance of the database using the Room.databaseBuilder() method and accessing DAO methods through the database instance.

Example usage:

Data entity:

java code

`@Entity public class User {     @PrimaryKey     public int uid;          @ColumnInfo(name = "first_name")     public String firstName;          @ColumnInfo(name = "last_name")     public String lastName;          // Constructors, getters, and setters }`

Data access object (DAO):

`@Dao public interface UserDao {     @Query("SELECT * FROM user")     List<User> getAll();      @Query("SELECT * FROM user WHERE uid IN (:userIds)")     List<User> loadAllByIds(int[] userIds);      @Query("SELECT * FROM user WHERE first_name LIKE :first AND " +            "last_name LIKE :last LIMIT 1")     User findByName(String first, String last);      @Insert     void insertAll(User... users);      @Delete     void delete(User user); }`

Database:

`@Database(entities = {User.class}, version = 1) public abstract class AppDatabase extends RoomDatabase {     public abstract UserDao userDao(); }`

Usage:

`AppDatabase db = Room.databaseBuilder(         applicationContext,         AppDatabase.class, "database-name" ).build();  UserDao userDao = db.userDao(); List<User> users = userDao.getAll();`


[Defining entities in Room](https://developer.android.com/training/data-storage/room/defining-data)
- When using the Room persistence library in Java, entities are used to represent the objects that you want to store in the database.
- Each entity is defined as a class annotated with `@Entity`.
- An entity class includes fields for each column in the corresponding database table.
- The `@PrimaryKey` annotation is used to define the primary key for an entity.
- Room uses the class name as the default table name, but you can customize it using the `tableName` property of the `@Entity` annotation.
- You can specify custom column names using the `@ColumnInfo` annotation.
- Composite primary keys can be defined by listing multiple columns in the `primaryKeys` property of the `@Entity` annotation.
- Fields that should not be persisted can be annotated with `@Ignore`.
- Room supports full-text search (FTS) using the `@Fts3` or `@Fts4` annotations for FTS-enabled tables.
- Indices can be added to specific columns using the `@Index` annotation within the `@Entity` annotation.
- Unique constraints can be enforced on columns using the `unique` property of the `@Index` annotation.
- Java-based immutable value classes annotated with `@AutoValue` can be used as entities in Room 2.1.0 and higher.
- Abstract methods in `@AutoValue` classes can be annotated with `@PrimaryKey`, `@ColumnInfo`, `@Embedded`, and `@Relation` using `@CopyAnnotations`.

[Related entities in Room](https://developer.android.com/training/data-storage/room/relationships)












![[Pasted image 20230529111319.png]]

[Accessing data with Room](https://developer.android.com/training/data-storage/room/accessing-data#java)

## Questions

1. What database engine is Room wrapped around? Do you think this is a good choice? Why or why not?
	1. Room is built on top of SQLite, which is a widely used open-source relational database engine.
	2. the why is that SQLite is Lightweight and Embedded: SQLite is designed to be lightweight and embedded within applications, making it a suitable choice for mobile apps or applications with limited resources. It doesn't require a separate database server process, and the entire database is contained within a single file.
2. Do Rooms have any similarities to JPA?
	1. Yes, Room and JPA (Java Persistence API) have some similarities in their goals and functionality. Both Room and JPA are frameworks that provide object-relational mapping (ORM) capabilities in Java for working with databases. They aim to simplify the process of storing and retrieving data from a database using object-oriented principles.
3. Describe a DAO in your own words
	1. the DAO allows you to access your database without having to write SQL. This enables separation of concerns! 