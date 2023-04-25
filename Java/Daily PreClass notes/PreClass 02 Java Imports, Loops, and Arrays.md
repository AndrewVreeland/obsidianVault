[Java Imports](https://www.programiz.com/java-programming/packages-import)

1.  Use an analogy to explain Built-In packages. Give examples.
	1. These packages come with the JDK and are not user created. 
2.  Explain the steps for creating a new package in IntelliJ.
	1. To define a package in Java, you use the keyword `package`.

`package packageName;

Java uses file system directories to store packages. Let's create a Java file inside another directory.

For example:

└── `com
  └──`` test
    └──`` Test.java

Now, edit **Test.java** file, and at the beginning of the file, write the package statement as:

`package com.test;

Here, any class that is declared within the test directory belongs to the **com.test** package.

Here's the code:

`package com.test;

`class Test {
 ``   public static void main(String[] args){
   ``     System.out.println("Hello World!");
    ``}
``}

**Output**:

`Hello World!

Here, the Test class now belongs to the **com.test** package.

[Different types of loops in Java](https://www.baeldung.com/java-loops)

1.  Which loop types use a loop counter?
	2. For loop, For Each loop
2.  Explain the difference between While and Do-While loops.
	1. it repreats a statement or a block of statements while its controlling boolean equates to true. 
[Java Arrays](https://www.tutorialspoint.com/java/java_arrays.htm)

1.  Describe 3 built-in methods for Arrays.
	1. **public static int binarySearch(Object[] a, Object key)**
		1. Searches the specified array of Object ( Byte, Int , double, etc.) for the specified value using the binary search algorithm. The array must be sorted prior to making this call. This returns index of the search key, if it is contained in the list; otherwise, it returns ( – (insertion point + 1)).



2. **public static boolean equals(long[] a, long[] a2)**
	1. Returns true if the two specified arrays of longs are equal to one another. Two arrays are considered equal if both arrays contain the same number of elements, and all corresponding pairs of elements in the two arrays are equal. This returns true if the two arrays are equal. Same method could be used by all other primitive data types (Byte, short, Int, etc.)

3. **public static void fill(int[] a, int val)**
	1. Assigns the specified int value to each element of the specified array of ints. The same method could be used by all other primitive data types (Byte, short, Int, etc.)

4. **public static void sort(Object[] a)**
	1. Sorts the specified array of objects into an ascending order, according to the natural ordering of its elements. The same method could be used by all other primitive data types ( Byte, short, Int, etc.)
5.  How is the size of an array determined in Java?
	1. you have to manually determine the size in java Ex. `double[] myList = new double[10];