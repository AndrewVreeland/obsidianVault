## Gradle 
- Build Settings
- Gradle init - used in command line to create new project
	- Gradle must live in its own file AKA its own root.
- Other options
	- Maven
- Need to run intellij from the Gradle root where the SETTINGS.GRADLE LIVES

## Intellij

- IDE: Intergrated Developer Enviornement
- commandline shortcut: idea .
- easiest way to check your Java Version AKA SDK 
- Interface
	- code/project tabs
	- gradle tabs
	- terminal tabs/run output
- Debugger



## Testing
- minimizes Bugs
- Junit Jupiter TESTING SWEET 
- Test Pattern
	- Arrange
	- Act 
	- Assert
-  class Library {

``@Test void nameOfFunctionReturnsTrue(){
``	Library classUnderTest = new Library();
``	assertFalse( condition: classUnderTest.someLibraryMethod(), message: "someLibraryMethod should return 'true' ")
`` }

@Test void returnPassedNumberReturnedPassedValue(){
 Arrange (our data)
 `Library sut = new Library();
 `int returnedValue;
 Act (upon our data`
 `returnedValue = sut.returnPAssedNumber (number: 10)
 Assert (our expected value)`
 `assertEquals(expected:10, actual: returnedValue);
`}

``}`
## ArrayLists vs Arrays
1. ArrayLists
	1. mutable length (can get longer)
	2. .get() in order to access the index
	3. ArrayList<Integer> myArr = new ArrayList<>
	4.  Integer with a capital I are objects not primitives compared to the int in a regular Array.
2. Arrays
	1. immutable length (can not get longer)
	2. arr[0] in order to access the index of an array
	3. int[] myArr = new int[5];



