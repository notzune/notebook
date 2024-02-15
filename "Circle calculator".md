[Link to Video Tutorial](https://youtu.be/e0EdRM-i6bk)

```java
public class Circle {

}
```

okay so you are given this empty "Circle" [[Class (computer programming)|class]] and are tasked with a couple of things[^1]:

1. you need to create a [[Accessors and mutators|getter]] and [[Accessors and mutators|setter]] for the radius
2. a "CalculateArea" [[Function (computer programming)#Definition of a Method ( Object-Oriented Programming OOP )|method]] that calculates and [[Return statement|returns]] the calculated [[Circle#Area|circle area]]
3. a "CalculateCircumference" method that calculates and returns the calculated [[Circle#Circumference|circle circumference]]

from this prompt we can infer two we will need:

1. an [[Instance variable|instance variable]] that is a `double` 
	1. since we will be doing math with it later so it makes sense to store it as a number
	2. we will call this variable `radius` since we will need to make a setter and getter for it later
	3. see also: [[Double (data type)|double (data type)]]
2. we will make a constructor that takes a parameter so that we can quickly set its state when we [[Instance (computer programming)|instantiate]] it without having to remember to set it ourselves.
		1. i know that the instructions ask for a default (no parameter) constructor, but that's kind of pointless especially since it goes against well established coding principles
		2. it's better practice to have a constructor that initializes the instance variables with the object, there's a [quora post](https://www.quora.com/Do-I-have-to-call-a-default-constructor-in-Java-as-a-common-practice#:~:text=A%20default%20constructor%2C%20i.e.%20one,(hence%20%E2%80%9Edefault%E2%80%9C).) that explains why it's better to design something this way, and personally i think this is best practice, i'll probably talk about it more when I explain [[SOLID]]
3. we also know that our get and set methods should [[Return type|return]] and pass a `double`, respectively.
4. we also know that since we are calculating things, we first want to double check the formula for whatever we are calculating (this is where math is important in programming) and we can assume we will be using the Java `Math` package.
	1. it's good that whenever you are using an [[Application programming interface (API)|API]] like the Math package or anything that you are importing really, it is good to check their [[Program documentation|documentation]] (usually in the form of [[Javadoc|javadocs]] in the context of java programs). [here is the link to the javadocs for the Math package](https://docs.oracle.com/javase/8/docs/api/java/lang/Math.html).

now that we know all of that we can start working on the class

```java
package xyz.zuner.tutorial;

public class Circle {

	// private access modifier because only this class (object) should be able to see it
	private double radius;

	// constructor, here we want to pass the starting radius to initialize it
	public Circle(double r) {
		this.radius = r;
	}

	// let's make our getters and setters now

	// getter
	// double return type
	// public because it is an accessor
	public double getRadius() {
		return radius;
	}

	// setter
	// void because we aren't returning anything
	// public because it is a mutator
	// pass a variable (the new radius)
	public void setRadius(double r) {
		this.radius = r;
	}

	// now we want to calculate area and circumference
	// area = pi * r^2
	// circumference = 2 * pi * r
	// returns the values as doubles
	
	public double calculateCircumference() {
		return 2 * Math.PI * radius;
	}

	public double calculateArea() {
		return Math.PI * Math.pow(radius, 2.0);
	}

	// finally let's make a toString method to quickly show radius
	public String toString() {
		return "Radius: " + radius;
	}
}
```

now let's implement this class into our main method

```java
package xyz.zuner.tutorial;

// main class
public class ExampleClass {

	// main method
	public static void main(String[] args) {
		// instantiate two new `Circle` objects
		Circle c1 = new Circle(5); // let's set its radius to 5
		Circle c2 = new Circle(10); // let's set this one to 10

		// let's get their radius and print it out
		System.out.println("Radius of circle 1: " + c1.getRadius());
		System.out.println("Radius of circle 2: " + c2.getRadius());

		// alternatively we can use the `toString()` method
		System.out.println(c1.toString());
		System.out.println(c2.toString());

		// let's also calculate their circumferences and areas

		// circle 1:
		System.out.println("Circumference of circle 1: " + c1.calculateCircumference());
		System.out.println("Area of circle 1: " + c1.calculateArea()));

		// circle 2:
		System.out.println("Circumference of circle 2: " + c2.calculateCircumference());
		System.out.println("Area of circle 2: " + c2.calculateArea()));

		// now let's change their radiuses

		c1.setRadius(20); // change circle 1's radius to 20
		c2.setRadius(30); // change circle 2's radius to 30

		// let's get their NEW radius and print it out
		System.out.println("New radius of circle 1: " + c1.getRadius());
		System.out.println("New radius of circle 2: " + c2.getRadius());

		// now let's calculate their NEW circumferences and areas

		// circle 1:
		System.out.println("New circumference of circle 1: " + c1.calculateCircumference());
		System.out.println("New area of circle 1: " + c1.calculateArea()));

		// circle 2:
		System.out.println("New circumference of circle 2: " + c2.calculateCircumference());
		System.out.println("New area of circle 2: " + c2.calculateArea()));
	}
}
```
[^1]:  the instructions also say to create a constructor that doesn't take a parameter, but i explain why this is a bad idea