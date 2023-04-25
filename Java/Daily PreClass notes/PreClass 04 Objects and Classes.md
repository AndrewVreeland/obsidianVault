## [Java OO Tutorial (only the Object and Class ones)](https://docs.oracle.com/javase/tutorial/java/concepts/)

1.  Explain the difference between an object and a class.
	1. A class is a blueprint from which objects are created where Objects are software bundles of related state and data.
2.  Name two types of state that a Student object might have.
	1. you could have the state of an object have values that change based on user input
	2. you could also have state change based on a timer.
3.  Name two types of behaviours that a student object might have.
	1. you could have an on off behaviour 
	2. or you could have something like a search or a find method that changes state based on what is recieved.

## [Java Classes (do NOT do the Nested Classes section)](https://docs.oracle.com/javase/tutorial/java/javaOO/classes.html)

#Class EX. 
public class #Bicycle {
        
    // **the Bicycle class has**
    // **three _fields_**
    public int cadence;
    public int gear;
    public int speed;
        
    // **the Bicycle class has**
    // **one _constructor_**
    public Bicycle(int startCadence, int startSpeed, int startGear) {
        gear = startGear;
        cadence = startCadence;
        speed = startSpeed;
    }
        
    // **the Bicycle class has**
    // **four _methods_**
    public void setCadence(int newValue) {
        cadence = newValue;
    }
        
    public void setGear(int newValue) {
        gear = newValue;
    }
        
    public void applyBrake(int decrement) {
        speed -= decrement;
    }
        
    public void speedUp(int increment) {
        speed += increment;
    }
        
}
#SubClass EX.
public class MountainBike extends Bicycle {
        
    // **the MountainBike subclass has**
    // **one _field_**
    public int seatHeight;

    // **the MountainBike subclass has**
    // **one _constructor_**
    public MountainBike(int startHeight, int startCadence,
                        int startSpeed, int startGear) {
        super(startCadence, startSpeed, startGear);
        seatHeight = startHeight;
    }   
        
    // **the MountainBike subclass has**
    // **one _method_**
    public void setHeight(int newValue) {
        seatHeight = newValue;
    }   

}
#Class_Declarations
In general, class declarations can include these components, in order 

1.  Modifiers such as _public_, _private_, and a number of others that you will encounter later. (However, note that the _private_ modifier can only be applied to [Nested Classes](https://docs.oracle.com/javase/tutorial/java/javaOO/nested.html).)
2.  The class name, with the initial letter capitalized by convention.
3.  The name of the class's parent (superclass), if any, preceded by the keyword _extends_. A class can only _extend_ (subclass) one parent.
4.  A comma-separated list of interfaces implemented by the class, if any, preceded by the keyword _implements_. A class can _implement_ more than one interface.
5.  The class body, surrounded by braces, {}.

## Objects

An object is a software of related stated and behavior

Objects have _state_ and _behavior_

The software object’s state is stored in #fields (aka variables in some languages) and the behavior is exposed thorough _methods_ (aka functions in some languages)

#Methods operate based off the state and is the primary way objects talk to each other.

#data_encapsulation is when the state is hidden and all interaction happens through the methods

The benefits of using objects include:

-   Modularity
-   Information-hiding
-   Code re-use
-   Plug-and-play and Easy Debugging

## Declaring Member Variables 

#### There are several kinds of variables:

-   Member variables in a class—these are called #fields.
-   Variables in a method or block of code—these are called _local variables_.
-   Variables in method declarations—these are called _parameters_.

`The` #Bicycle `class uses the following lines of code to define its` #fields:

public int cadence;
public int gear;
public int speed;

#### Field declarations are composed of three components, in order:

1.  Zero or more modifiers, such as `public` or `private`.
2.  The field's type.
3.  The field's name.

The #fields of #Bicycle are named `cadence`, `gear`, and `speed` and are all of data type #integer (`int`). The #public keyword identifies these fields as public members, accessible by any #object that can access the class.

## Access Modifiers

The first (left-most) modifier used lets you control what other classes have access to a member field. For the moment, consider only #public and #private`. Other access modifiers will be discussed later.

-   #public modifier—the field is accessible from all classes.
-   #private modifier—the field is accessible only within its own class.

**Defining Methods:**

Required Elements in Methods Declaration

-   return type, name, parens (), and a body between braces {}
    
-   Six Components of Method Declaration:
    1.  Modifiers
    2.  Return type
    3.  Method Name
    4.  Parameter list in parens
    5.  Exception List
    6.  Method body in braces
-   a method signature is the method’s name an parameter type

**Naming a Method:**

method names should be a VERB or a multi-word name that begins with a verb in

a method has unique names within a class

**Overloading Methods:**

Methods in a class can have the same names if desired but only if they have different parameters

A method with the same name and the same number and type of arguments cannot be declared because the complier will not be able to differentiate between the two; this creates a compile-time error

The complier does not consider return type when differentiating between methods

**Providing Constructors for Classes:**

A class has constructors that are invoked to create objects from the class blueprint.

Constructor declarations look similar to method declarations with the exception of using the class name and have no return type

**Passing Information to a Methods or a Constructor:**

The declaration for a method or constructor determines the number and type of arguments for themselves.





7.  Explain the significance of a constructor for a class.
	1. constructors are sued to create objects from the class blueprint
8.  Write the declaration statement for a class named “Student” (do not fill it with fields and methods).
	1. public static class Student {
	
			}

## [Binary, Decimal and Hexadecimal Numbers](https://www.mathsisfun.com/binary-decimal-hexadecimal.html)

1.  What is the value of the binary number 1101?
	1. D
2.  Write the number 52 in binary. Write it in hexidecimal.
	1. 0101, 0001