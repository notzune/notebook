# Chapter 9: Inheritance

[[Inheritance (object-oriented programming)|inheritance]] allows one class to inherit the fields and methods of another. this is fundamental for achieving code reusability and establishing a hierarchy of class relationships.

- **Interface**: a contract that specifies a set of methods that implementing classes must have.
- **Parent Class (Superclass)**: the class whose properties and methods are inherited by another class.
- **Derived Class (Subclass)**: the class that inherits from the parent class.

**Keywords/Classes**:

- `abstract`: used to declare either a method without implementation or a class that cannot be instantiated.
- `extends`: used by a class to inherit another class.
- `implements`: used by a class to adhere to interfaces.
- `private`, `protected`, `public`: [[Access modifier|access modifiers]] that control the visibility of fields and methods.
- `super`: used to refer to parent class objects or to call the superclass constructor.
- `Object`: the root class from which every class in Java implicitly inherits

```java
// define a base class called Vehicle
class Vehicle {
  private String brand;

  // constructor for Vehicle
  Vehicle(String brand) {
    this.brand = brand;
  }

  // method to display the brand of the vehicle
  void displayBrand() {
    print("Brand: " + brand);
  }
}

// define a derived class called Car that extends Vehicle
class Car extends Vehicle {
  private int numWheels;

  // constructor for Car
  Car(String brand, int numWheels) {
    super(brand); // Call the superclass constructor
    this.numWheels = numWheels;
  }

  // method to display the details of the car
  void displayDetails() {
    super.displayBrand(); // call the superclass method
    print("Number of wheels: " + numWheels);
  }
}
```

# Chapter 10: Polymorphism

[[Polymorphism (computer science)|polymorphism]] is the ability of an object to take on many forms, allowing methods to do different things based on the object on which they are called.

- **Polymorphic Reference/Variable**: a variable that can refer to objects of different types at different times.
- **Overriding**: a feature that allows a subclass to provide a specific implementation of a method that is already provided by its superclass.

**Key Concepts**:

- **Late Binding (Dynamic Binding)**: the type of the object is determined at runtime.
- **Inheritance & Interfaces**: essential for polymorphism, as they allow objects to be treated as instances of their parent classes or interfaces.

```java
// define an interface Shape with a method draw
interface Shape {
  void draw();
}

// implement Shape with a Rectangle class
class Rectangle implements Shape {
  void draw() {
    print("Drawing a rectangle");
  }
}

// implement Shape with a Circle class
class Circle implements Shape {
  void draw() {
    print("Drawing a circle");
  }
}

// a function that uses polymorphic references to draw shapes
void drawShapes(List<Shape> shapes) {
  for (Shape shape : shapes) {
    shape.draw(); // polymorphic call
  }
}
```

in this example, the method ``draw()`` changes its output based on the `Shape` object (an object that implements the `Shape` interface, such as `Rectangle` or `Circle`).

# Chapter 11: Exceptions

java uses exceptions to handle errors and other exceptional events. exceptions can broadly be classified into two main categories: **checked exceptions** and **unchecked exceptions**.

- **Checked Exception**: an exception that must be either caught or declared in the method signature.
- **Unchecked Exception**: an exception that does not need to be explicitly handled (e.g., `RuntimeExceptions`).
- **Stack Trace**: a report of the active stack frames at a certain point in time during the execution of a program.

**Keywords/Classes**:

- `try/catch`: blocks used to handle exceptions.
- `throw`: used to explicitly throw an exception.
- `throws`: declares an exception, alerting the compiler that this exception might be thrown by the method.
- `Exception`, `ArithmeticException`, `NumberFormatException`, `StringIndexOutOfBoundsException`: various exception classes provided by Java.

## 1. `Exception`

the `Exception` class is a superclass of all checked exceptions in Java. it is also the parent class for many unchecked exceptions. exceptions that are derived from the `Exception` class (other than `RuntimeException` and its subclasses) are checked exceptions, meaning they need to be either caught within a try-catch block or declared to be thrown in the method signature using the `throws` keyword. When you encounter an `Exception`, it typically indicates that a condition has occurred that the application might want to recover from.

**common use**: it is often extended to create custom exceptions specific to an application's needs.

## `ArithmeticException`

this is an unchecked exception and a subclass of `RuntimeException`. it indicates exceptional conditions associated specifically with arithmetic operations.

**when it happens**: the most common cause of an `ArithmeticException` is dividing an integer by zero. it can also occur in other erroneous arithmetic conditions, such as integer overflow during an operation.
### ArithmeticException

```java
// method to perform division and handle possible exceptions
void divide(int numerator, int denominator) {
  try {
    if (denominator == 0) {
      throw new ArithmeticException("Cannot divide by zero");
    }
    int result = numerator / denominator;
    print("Result: " + result);
  } catch (ArithmeticException e) {
    print("Error occurred: " + e.getMessage());
  }
}
```
## IOException

```java
// method to read a file that might throw an IOException
void readFile(String filePath) throws IOException {
  try {
    // attempt to open and read the file
    openFile(filePath);
    print("File read successfully");
  } catch (IOException e) {
    // handle the situation where the file could not be read
    print("Error reading file: " + e.getMessage());
    // optionally re-throw the exception
    throw e;
  }
}
```

## NullPointerException

```java
// method to access a member of an object that might be null
void printLength(String s) {
  try {
    int length = s.length();
    print("Length of the string: " + length);
  } catch (NullPointerException e) {
    print("String is null!");
  }
}
```

## `NumberFormatException`

`NumberFormatException` is another unchecked exception and a subclass of `RuntimeException`. it occurs when an application attempts to convert a string into one of the numeric types (`byte`, `short`, `int`, `long`, `float`, or `double`) but the string does not have the appropriate format.

**when it happens**:

- trying to parse a string that contains non-numeric characters where a number is expected.
- parsing strings that represent numbers outside the range of the target number type.

**example**:

```java
String number = "abc"; int result = Integer.parseInt(number);  
// will throw NumberFormatException`
```
### NumberFormatException

```java
// method to parse a string into an integer
void parseInteger(String numberStr) {
  try {
    int number = Integer.parseInt(numberStr);
    print("Parsed number: " + number);
  } catch (NumberFormatException e) {
    print("Invalid number format: " + numberStr);
  }
}
```

## `StringIndexOutOfBoundsException`

this is also an unchecked exception and a subclass of `IndexOutOfBoundsException`. it specifically occurs when an attempt is made to access an index of a string that is either negative or greater than or equal to the length of the string.

**when it happens**:

- accessing a character at a negative index.
- accessing a character at an index equal to or greater than the length of the string.

```java
String text = "hello";
char ch = text.charAt(5);  
// will throw StringIndexOutOfBoundsException because valid indexes are 0-4
```
### String Index Out of Bounds Exception

```java
// Method to get a character from a string safely
void getCharacter(String str, int index) {
  try {
    char character = str.charAt(index);
    print("Character at index " + index + ": " + character);
  } catch (StringIndexOutOfBoundsException e) {
    print("Index out of bounds for string length " + str.length());
  }
}
```

## Array Out of Bounds Exception

```java
// method to access an array element safely
void accessArrayElement(int[] array, int index) {
  try {
    int element = array[index];
    print("Element at index " + index + ": " + element);
  } catch (ArrayIndexOutOfBoundsException e) {
    print("Index out of bounds: " + index);
  }
}
```
# Chapter 12: Recursion

[[Recursion|recursion]] involves methods that call themselves in order to solve a problem by breaking it down into simpler, smaller versions of the same problem. this approach can simplify the code, especially when working with problems that can naturally be divided into similar subproblems. The key components of a recursive function are:

1. **Base Case**: this is the condition under which the function will stop calling itself. Without a proper base case, a recursive function may lead to infinite recursion, causing a stack overflow error.
2. **Recursive Case**: this is the part of the function where it calls itself with modified parameters to bring it closer to the base case.

## Advantages of Recursion

- it simplifies the code for problems related to trees, graphs, combinations, and permutations.
- recursion is integral in divide and conquer strategies like `mergesort` and `quicksort`.

## Disadvantages of Recursion

- recursive functions can be memory intensive and slower due to overheads of function calls and returns.
- they can lead to stack overflow if the depth of recursion becomes too large.

here are some pseudo code examples of common recursive problems to illustrate how recursion works.

```java
// nethod to calculate factorial using recursion
int factorial(int n) {
  if (n == 0) { // base case
    return 1;
  } else { // recursive case
    return n * factorial(n - 1);
  }
}

// example usage:
int result = factorial(5);
print("Factorial: " + result);
```

```java
// recursive method to find the nth Fibonacci number
function fibonacci(n) {
  if (n <= 1) {  // base cases: fib(0) = 0, fib(1) = 1
    return n;
  } else {       // recursive case: fib(n-1) + fib(n-2)
    return fibonacci(n - 1) + fibonacci(n - 2);
  }
}

// example usage:
output = fibonacci(7);
print(output);  // outputs 13
```

```java
// recursive method to perform binary search on a sorted array
function binarySearch(array, target, low, high) {
  if (low > high) {  // base case: target not found
    return -1;
  }

  mid = (low + high) / 2;
  if (array[mid] == target) {  // target found
    return mid;
  } else if (target < array[mid]) {  // search the left half
    return binarySearch(array, target, low, mid - 1);
  } else {  // search the right half
    return binarySearch(array, target, mid + 1, high);
  }
}

// example usage:
array = [1, 2, 3, 4, 5, 6, 7, 8, 9];
target = 4;
result = binarySearch(array, target, 0, array.length - 1);
print("Index of " + target + ": " + result);  // outputs: index of 4: 3
```