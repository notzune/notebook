the main method is a special [[Function (computer programming)#Definition of a Method ( Object-Oriented Programming OOP )|method]] in some [[Object-Oriented Programming|OOP]] [[Programming language|languages]] such as [[Java]] where the [[Compiler|compiler]] (or in this case the [[Java Virtual Machine (JVM)|JVM]]) knows where to begin to execute your [[Logic (computer programming)|logic]] for the [[Computer program|program]] to actually run.

you can think of it as an entry-point into your program, where the [[Method body (object-oriented programming)|method body]] tells the host [[Computer|machine]] what to do.

in Java, the main method will always[^1] look like this:

```java
public static void main(String[] args) {

	// method body gets executed
}
```

the main method is usually where you [[Instance (computer programming)|instantiate]] your [[Object (computer science)|objects]] and [[Class (computer programming)|classes]] in-order to call their methods.

[^1]: there are cases where it might not look like this such as when working with certain [[Application programming interface (API)|APIs]].