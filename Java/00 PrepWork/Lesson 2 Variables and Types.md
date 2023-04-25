[[Lesson 3 Conditionals]]
-   `byte` (number, 1 byte)
-   `short` (number, 2 bytes)
-   `int` (number, 4 bytes)
-   `long` (number, 8 bytes)
-   `float` (float number, 4 bytes)
-   `double` (float number, 8 bytes)
-   `char` (a character, 2 bytes)
-   `boolean` (true or false, 1 byte)

## How to declare different types

### numbers

1. int myNumber;
		myNumber =5;
2. double dD = 4.5;
		dD = 3.0;
3. float f = (float) 4.5; OR float f = 4.5f  `(f is a shorter way of casting float)

## Characters and Strings

1. char c = 'g';

2. A string is a real type you can create a string with a constructor like this,
		* String s1 = new String("Who let the dogs out?"); `String object stored in heap memory
		* String s2 = "Who who who who!"; `String literal stored in String pool
		* you can concat the different strings like this! 
				* string s3 = s1 +s2

## boolean 
`every comparison operator in java will return the type boolean. Unlike other languages, it only accepts two special values: `true` or `false`

1. EX 
boolean b = false;
b = true;

boolean toBe = false;
b = toBe || !toBe;
if (b) {
    System.out.println(toBe);
}

int children = 0;
b = children; // Will not work
if (children) { // Will not work
    // Will not work
}

int a;
boolean b = true; 
boolean c = false; 
a = b + c;            //The following line will give an error
System.out.println(a);

