[[Lesson 4 Arrays]]
Java uses boolean variables to evaluate conditions. The boolean values `true` and `false` are returned when an expression is compared or evaluated. For example:

```java
int a = 4;

if (a == 4) {
    System.out.println("Ohhh! So a is 4!");
}
```

## Boolean operators
There aren't that many operators to use in conditional statements and most of them are pretty straight forward:
```java
int a = 4;
int b = 5;
boolean result;
result = a < b; // true
result = a > b; // false
result = a <= 4; // a smaller or equal to 4 - true
result = b >= 6; // b bigger or equal to 6 - false
result = a == b; // a equal to b - false
result = a != b; // a is not equal to b - true
result = a > b || a < b; // Logical or - true
result = 3 < a && a < 6; // Logical and - true
result = !result; // Logical not - false
```

## if - else and between
The if, else statement in Java is pretty simple.

```java
if (a == b) {
    // a and b are equal, let's do something cool
}
```

And we can also add an else statement after an if, to do something if the condition is not true

```java
if (a == b) {
    // We already know this part
} else {
    // a and b are not equal... :/
}
```

The if - else statements doesn't have to be in several lines with {}, if can be used in one line, or without the {}, for a single line statment.

```java
if (a == b)
    System.out.println("Another line Wow!");
else
    System.out.println("Double rainbow!");
```

There is a another way to write a one line if - else statement by using the operator ? :

```java
int a = 4;
int result = a == 4 ? 1 : 8;

// result will be 1
// This is equivalent to
int result;

if (a == 4) {
    result = 1;
} else {
    result = 8;
}
```

## == and equals

The operator `==` works a bit different on objects than on primitives. When we are using objects and want to check if they are equal, the operator `==` will say if they are the same, if you want to check if they are logically equal, you should use the `equals` method on the object. For example:

```java
String a = new String("Wow");
String b = new String("Wow");
String sameA = a;

boolean r1 = a == b;      // This is false, since a and b are not the same object
boolean r2 = a.equals(b); // This is true, since a and b are logically equals
boolean r3 = a == sameA;  // This is true, since a and sameA are really the same object
```