[Primitives vs. Objects](https://www.baeldung.com/java-primitives-vs-objects)

1.  Explain the difference between an “int” and an “Integer” in Java.
	1. the space in memory that they take up, int takes up far less space then Integer. int is a primitive where Intiger is a reference type
2.  What is the default value for ints? Integers?
	1. for ints AKA primitive types is 0 and Integers is null because they are a wrapper class? 
3.  What is autoboxing? Unboxing?
	1. The process of converting a primitive type to a reference one is called autoboxing, the opposite process is called unboxing.

[Exceptions in Java (read the first three sections on the left: What is an Exception, The Catch or Specify Requirement, Catching and Handling Exceptions)](https://docs.oracle.com/javase/tutorial/essential/exceptions/index.html)

1.  List the three basic categories of exceptions.
	1. _checked exception_, If the user were to try to creat a file with the same name as another file on your windows computer and the computer will throw a pop up error which is from a program set to check those variables. 
	2. _error_, These are exceptional conditions that are external to the application, and that the application usually cannot anticipate or recover from.
	3.  _runtime exception_, These are exceptional conditions that are internal to the application they includde logic errors or improper use of an API.
2.  What type of statement can you use to handle an exception?
	1. you can use a try catch statement to catch and handle those errors.

[Using Scanner to read in a file in Java](https://docs.oracle.com/javase/tutorial/essential/io/scanning.html)

1.  Describe a situation where you think it would be useful to have a program that scans text.
	1. One situation where it would be useful to have a program that scans text in Java is in a news aggregation system. This system collects news articles from various sources and needs to automatically categorize and tag them for further processing or display on a website or app.
2.  What is input from a Scanner broken down into?
	1. In Java, the input from a `Scanner` object is broken down into tokens, which are discrete units of text that are separated by delimiters. A delimiter is a special character or a pattern that is used to split the input text into smaller chunks.