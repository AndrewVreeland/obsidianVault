## Reading

[Java Basics](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/index.html)

1.  What does “strong typed” mean?
	1. Java is considered strongly typed because **it demands the declaration of every variable with a data type**.
2.  What are the primitive data types?
	-   **byte**: The `byte` data type is an 8-bit signed two's complement integer. It has a minimum value of -128 and a maximum value of 127 (inclusive). The `byte` data type can be useful for saving memory in large [arrays](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/arrays.html), where the memory savings actually matters. They can also be used in place of `int` where their limits help to clarify your code; the fact that a variable's range is limited can serve as a form of documentation.
    
	-   **short**: The `short` data type is a 16-bit signed two's complement integer. It has a minimum value of -32,768 and a maximum value of 32,767 (inclusive). As with `byte`, the same guidelines apply: you can use a `short` to save memory in large arrays, in situations where the memory savings actually matters.
    
	-   **int**: By default, the `int` data type is a 32-bit signed two's complement integer, which has a minimum value of -231 and a maximum value of 231-1. In Java SE 8 and later, you can use the `int` data type to represent an unsigned 32-bit integer, which has a minimum value of 0 and a maximum value of 232-1. Use the Integer class to use `int` data type as an unsigned integer. See the section The Number Classes for more information. Static methods like `compareUnsigned`, `divideUnsigned` etc have been added to the [`Integer`](https://docs.oracle.com/javase/8/docs/api/java/lang/Integer.html) class to support the arithmetic operations for unsigned integers.
    
	-   **long**: The `long` data type is a 64-bit two's complement integer. The signed long has a minimum value of -263 and a maximum value of 263-1. In Java SE 8 and later, you can use the `long` data type to represent an unsigned 64-bit long, which has a minimum value of 0 and a maximum value of 264-1. Use this data type when you need a range of values wider than those provided by `int`. The [`Long`](https://docs.oracle.com/javase/8/docs/api/java/lang/Long.html) class also contains methods like `compareUnsigned`, `divideUnsigned` etc to support arithmetic operations for unsigned long.
    
	-   **float**: The `float` data type is a single-precision 32-bit IEEE 754 floating point. Its range of values is beyond the scope of this discussion, but is specified in the [Floating-Point Types, Formats, and Values](https://docs.oracle.com/javase/specs/jls/se7/html/jls-4.html#jls-4.2.3) section of the Java Language Specification. As with the recommendations for `byte` and `short`, use a `float` (instead of `double`) if you need to save memory in large arrays of floating point numbers. This data type should never be used for precise values, such as currency. For that, you will need to use the [java.math.BigDecimal](https://docs.oracle.com/javase/8/docs/api/java/math/BigDecimal.html) class instead. [Numbers and Strings](https://docs.oracle.com/javase/tutorial/java/data/index.html) covers `BigDecimal` and other useful classes provided by the Java platform.
    
	-   **double**: The `double` data type is a double-precision 64-bit IEEE 754 floating point. Its range of values is beyond the scope of this discussion, but is specified in the [Floating-Point Types, Formats, and Values](https://docs.oracle.com/javase/specs/jls/se7/html/jls-4.html#jls-4.2.3) section of the Java Language Specification. For decimal values, this data type is generally the default choice. As mentioned above, this data type should never be used for precise values, such as currency.
    
	-   **boolean**: The `boolean` data type has only two possible values: `true` and `false`. Use this data type for simple flags that track true/false conditions. This data type represents one bit of information, but its "size" isn't something that's precisely defined.
    
	-   **char**: The `char` data type is a single 16-bit Unicode character. It has a minimum value of `'\u0000'` (or 0) and a maximum value of `'\uffff'` (or 65,535 inclusive).

## Questions

1.  The term "instance variable" is another name for **non-static field**.
2.  The term "class variable" is another name for **static field**.
3.  A local variable stores temporary state; it is declared inside a **method**.
4.  A variable declared within the opening and closing parenthesis of a method is called a **parameter**.
5.  What are the eight primitive data types supported by the Java programming language? **byte, short, int, long, float, double, boolean, char**
6.  Character strings are represented by the class **java.lang.String**.
7.  An **array** is a container object that holds a fixed number of values of a single type.

## Compiling

As you may know, everything in a computer is represented by a series of 1's and 0's (which themselves represent high and low voltages on transistors, but that's a topic for another time). When the computer runs a program, the program itself is made of a bunch of 1's and 0's.

However, since we still need humans to write our programs, putting everything in 1's and 0's (called machine language) would be very difficult. So we made higher level languages like Java and C# to write code in. These languages look a lot more like English, so they're a lot easier to write and maintain.

When you compile code, the compilor (usually another program) takes the program the human wrote, and converts it into the program the computer can understand (i.e. converts from Java to machine language). The very short version could be, yes, compile means to make the code executable.

Something you may run into is people saying code does or does not compile. This means the compilor they used checks to make sure their program is written correctly according to the rules of the programming language. For example, most programming languages make you put a semicolon (;) at the end of every line. A very common mistake is to forget that semicolon, so when you try and compile the compilor gives you an error.

It's also important to note that just because the code compiles doesn't mean it works. It's sort of like how 3 + 4 < 5 is an equation that has the right form, but it is incorrect.


[XKCD: Compiling](https://xkcd.com/303/)

1.  Explain to a non-technical friend the difference in how compilation works in Java and JavaScript.
	- Java and JavaScript are both programming languages, but they are used in different ways and have different ways of handling code.

In Java, code is compiled, which means it goes through a process called compilation before it is executed. Compilation is like translating code from a language that humans can read and write, called source code, into a language that computers can understand, called machine code. The machine code is then executed by the computer's processor. Once Java code is compiled, the resulting compiled code, also known as bytecode, can be run on any device that has a Java Virtual Machine (JVM) installed, which acts as an interpreter to execute the bytecode.

On the other hand, JavaScript is an interpreted language. This means that JavaScript code is executed directly by the computer without going through a compilation step. When you load a webpage that contains JavaScript code in a web browser, the browser's built-in JavaScript engine interprets and executes the JavaScript code on the fly. This makes JavaScript a more flexible language that can be run on any device with a web browser, without the need for a separate compilation step.

In summary, the main difference in how compilation works in Java and JavaScript is that Java code is compiled into bytecode before execution, while JavaScript code is interpreted and executed directly by the computer. Java requires a Java Virtual Machine (JVM) to run, while JavaScript can run in any web browser that supports it.

2.  Does code complining mean that it works correctly?
	- no just because the code is compiling does not mean that it can function, here is a note that was listed above: It's also important to note that just because the code compiles doesn't mean it works. It's sort of like how 3 + 4 < 5 is an equation that has the right form, but it is incorrect.
[Reading Java Documentation](https://www.dummies.com/programming/java/making-sense-of-javas-api-documentation/)

1.  How many keywords does Java have?
	-  51 key words
2.  How do you print words to the console in Java?
	- **System.** **out.** **println("arbitrary text");