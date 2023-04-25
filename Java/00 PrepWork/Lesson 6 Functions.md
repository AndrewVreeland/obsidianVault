[[Lesson 7 Objects]]
In Java, all function definitions must be inside classes. We also call functions methods. Let's look at an example method

```java
public class Main {
    public static void foo() {
        // Do something here
    }
}
```

`foo` is a method we defined in class Main. Notice a few things about `foo`.

-   `static` means this method belongs to the class Main and not to a specific instance of Main. Which means we can call the method from a different class like that `Main.foo()`.
-   `void` means this method doesn't return a value. Methods can return a single value in Java and it has to be defined in the method declaration. However, you can use `return` by itself to exit the method.
-   This method doesn't get any arguments, but of course Java methods can get arguments as we'll see further on.

## Arguments 

Java methods are passed by value

By value means that arguments are copied when the method runs. Let's look at an example.

```java
public void bar(int num1, int num2) {
    ...
}
```

Here is a another place in the code, where bar is called

```java
int a = 3;
int b = 5;
bar(a, b);
```

You can picture in your head that when `bar(a, b)` is run, it's like in the beginning of `bar` the following two lines are written:

```java
int num1 = a;
int num2 = b;
```

And only then the rest of the method is run.

This means that `a` value get copied to `num1` and `b` value get copied to `num2`. Changing the values of `num1` and `num2` will not affect `a` and `b`.

If the arguments were objects, the rules remain the same, but it acts a bit differently. Here is a an example:

```java
public void bar2(Student s1, Student s2) {
    ...
}
```

And here is how we use it

```java
Student joe = new Student("joe");
Student jack = new Student("jack");
bar2(joe, jack);
```

Again we can picture the same two lines in the beginning of `bar2`

```java
Student s1 = joe;
Student s2 = jack;
```

But when we assign objects, it's a bit different than assigning primitives. `s1` and `joe` are two different references to the same object. `s1 == joe` is true. This means that running methods on `s1` will change the object `joe`. But if we'll change the value of `s1` as a reference, it will not affect the reference `joe`.

```java
s1.setName("Chuck"); // joe name is now Chuck as well
s1 = new Student("Norris"); // s1 is a new student, different than joe with the name of Norris
// s1 == joe   is not true anymore
```