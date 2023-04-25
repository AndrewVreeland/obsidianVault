## Reading

[Java OO Tutorial (review Object and Class, read the rest)](https://docs.oracle.com/javase/tutorial/java/concepts/)

1.  What is the difference between an #Object and a #Class in Java?
	1. an object is a software bundle where a class is a blueprint for objects to be created from.
2.  Explain to a non-technical friend the concept of #inheritance in Java.
	1. if bicycle is the class a mountain bike and road bike would be subclasess and inherit all of the things that are constant amoung all bikes such as two weels. to do this you have to use extends ex.
					class MountainBike **extends** Bicycle {

					    // new fields and methods defining 
					    // a mountain bike would go here }


[Java Static Keyword](https://www.programiz.com/java-programming/static-keyword)

## What is a static keyword in Java?

In Java, if we want to access class members, we must first create an #instance of the #class. But there will be situations where we want to access class members without creating any variables.

In those situations, we can use the #static keyword in Java. If we want to access class members without creating an instance of the class, we need to declare the class members static.

The `Math` class in Java has almost all of its members static. So, we can access its members without creating instances of the Math class. For example,

```
public class Main {
    public static void main( String[] args ) {

        // accessing the methods of the Math class
        System.out.println("Absolute value of -12 =  " + Math.abs(-12));
        System.out.println("Value of PI = " + Math.PI);
        System.out.println("Value of E = " + Math.E);
        System.out.println("2^2 = " + Math.pow(2,2));
    }
}
```

In the above example, we have not created any instances of the `Math` class. But we are able to access its methods: `abs()` and `pow()` and variables: `PI` and `E`.

It is possible because the methods and variables of the `Math` class are static.

1.  Static methods are also called what? Why?
	1. Class methods, because a static methods belong to the class rather than the object that it lives in.
2.  How can you access a variable of a class without instantiating an object from that class?
	1. by delcaring them static. 

### Example 1: Java static and non-static Methods

```
class StaticTest {

    // non-static method
    int multiply(int a, int b){
        return a * b;
    }

    // static method
    static int add(int a, int b){
        return a + b;
    }
}

public class Main {

   public static void main( String[] args ) {

        // create an instance of the StaticTest class
	    StaticTest st = new StaticTest();

        // call the nonstatic method
        System.out.println(" 2 * 2 = " + st.multiply(2,2));

        // call the static method
        System.out.println(" 2 + 3 = " + StaticTest.add(2,3));
   }
}
```


# Java #Singleton Class

## To create a Singleton Class 
	
-   Create a #private constructor of the class to restrict object creation outside of the class.
-   Create a `private` attribute of the class type that refers to the single object.
-   Create a #public #static method that allows us to create and access the object we created. Inside the method, we will create a condition that restricts us from creating more than one object.
- 
### Example: Java Singleton Class Syntax

```
class SingletonExample {

   // private field that refers to the object
   private static SingletonExample singleObject;
                                              
   private SingletonExample() {
      // constructor of the SingletonExample class
   }

   public static SingletonExample getInstance() {
      // write code that allows us to create only one object
      // access the object as per our need
   }
}
```

Singletons can be used while working with databases. They cam be used to create a connection pool to access the database while reuisng the same connection for all the clients. For Ex.

```
lass Database {
   private static Database dbObject;

   private Database() {      
   }

   public static Database getInstance() {

      // create object if it's not already created
      if(dbObject == null) {
         dbObject = new Database();
      }

       // returns the singleton object
       return dbObject;
   }

   public void getConnection() {
       System.out.println("You are now connected to the database.");
   }
}

class Main {
   public static void main(String[] args) {
      Database db1;

      // refers to the only object of Database
      db1= Database.getInstance();
      
      db1.getConnection();
   }
}
```

In our above example,

-   We have created a singleton class Database.
-   The dbObject is a class type field. This will refer to the object of the class Database.
-   The private constructor `Database()` prevents object creation outside of the class.
-   The static class type method `getInstance()` returns the instance of the class to the outside world.
-   In the Main class, we have class type variable db1. We are calling `getInstance()` using db1 to get the only object of the Database.
-   The method `getConnection()` can only be accessed using the object of the Database.
-   Since the Database can have only one object, all the clients can access the database through a single connection.


[Java Singleton Class](https://www.programiz.com/java-programming/singleton)

1.  What is a Design Pattern? Describe one or two with analogies from your previous work experience.
	1. A design pattern is like our code library that includes various coding techniques shared by programmers around the world.
2.  What is a Singleton?
	1. In Java, Singleton is a design pattern that ensures that a class can only have one object.




# What Is an #Interface?

 #objects define their interaction with the outside world through the #methods that they expose. Methods form the object's _interface_ with the outside world; the buttons on the front of your television set, for example, are the interface between you and the electrical wiring on the other side of its plastic casing. You press the "power" button to turn the television on and off.

In its most common form, an interface is a group of related methods with empty bodies. A bicycle's behavior, if specified as an interface, might appear as follows:

interface Bicycle {

    //  wheel revolutions per minute
    void changeCadence(int newValue);

    void changeGear(int newValue);

    void speedUp(int increment);

    void applyBrakes(int decrement);
}

To implement this interface, the name of your #class would change (to a particular brand of bicycle, for example, such as `ACMEBicycle`), and you'd use the #implements keyword in the class declaration:

class ACMEBicycle **implements** Bicycle {

    int cadence = 0;
    int speed = 0;
    int gear = 1;

   // The compiler will now require that methods
   // changeCadence, changeGear, speedUp, and applyBrakes
   // all be implemented. Compilation will fail if those
   // methods are missing from this class.

    void changeCadence(int newValue) {
         cadence = newValue;
    }

    void changeGear(int newValue) {
         gear = newValue;
    }

    void speedUp(int increment) {
         speed = speed + increment;   
    }

    void applyBrakes(int decrement) {
         speed = speed - decrement;
    }

    void printStates() {
         System.out.println("cadence:" +
             cadence + " speed:" + 
             speed + " gear:" + gear);
    }
}

Implementing an #interface allows a class to become more formal about the behavior it promises to provide. Interfaces form a contract between the class and the outside world, and this contract is enforced at build time by the compiler. If your class claims to implement an interface, all methods defined by that interface must appear in its source code before the class will successfully compile.

# What Is a Package?

A package is a namespace that organizes a set of related classes and interfaces. Conceptually you can think of packages as being similar to different folders on your computer. You might keep HTML pages in one folder, images in another, and scripts or applications in yet another. Because software written in the Java programming language can be composed of hundreds or _thousands_ of individual classes, it makes sense to keep things organized by placing related classes and interfaces into packages.


