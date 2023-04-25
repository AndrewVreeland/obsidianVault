## Example of a new JS file

Public class myClass{
public static void main(string[] args){

- <YOU CANT CALL FUNCTIONS HERE BECAUSE THIS IS A FUNCTION>
- you can only call on other functions here.
- public and static are modifiers, void is the return type and main is the entry point of the program.

}

public static string pluralized(){
This is a new Funciton

}

}

- You can import myClass into another JS file and then gain access to all of these functions. 
- You can not nest funcitons. each function has to live on its own.
- `static` - can be accessed without creating an instance of the class
   `void` - does not return anything
   `main` - the entry point of the program
   `System` - a pre-defined class in java that holds useful methods and variables
   `System.out` - a static variable within system that represents the standard output of the program
   `println` - a method that can be used to print a line

## Arrays

- int[] arr = {5} ---- this creates a new empty array with 5 memory spaces.
	- if you were to try to access the 6th location in the above array you would get an Index out of bounds.
	- 