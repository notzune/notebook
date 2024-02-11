```java
// import statements go at the top of the class
import java.util.bullshit;

// class header, public access modifier so any other class can see it
public class JavaExample {

	public final String SOME_STRING = "This is a constant!";

	// this is the main method, entry-point for the compiler
	public static void main(String[] args) {
		// here is where some logic goes
		
		// this method prints "Hey z!" to the console
		System.out.println("Hey z!");

		// we can assign a variable to return the output of a method
		String someVar = getSomeString();

		System.out.println(someVar); // then we can print it out
		// OUTPUT: This is a constant!

		// or we can reassing it like so
		someVar = getMethodString();

		System.out.printlin(someVar);
		// OUTPUT: This var can only b accessed in this method

		// we can do this since java runs code line by line
	}

	// private access modifier means only this class can run it
	// `String` return type which means expect a String obj returned
	private static String getMethodString() {
		// initialize a method variable
		String someString = "This var can only b accessed in this method";
		return someString;
	}

	// this is a public accessor method, a "getter"
	public static String getSomeString() {
		// this return the instance variable
		return SOME_STRING;
	}

	// not lets do a method with some "complex" logic
	// here you see its called "sumOfCubes"
	// and should do exactly that, sum the cubes of two numbers
	// since we pass things to it, it can't be static (since it changes)
	public double sumOfCubes(double val1, double val2) {
		// from the Math class in java
		double cubeVal1 = Math.pow(val1, 3.0);
		double cubeVal2 = Math.pow(val2, 3.0);

		double sum = cubeVal1 + cubeVal2;
		return sum;

		// alternatively, you can just do
		// return cubeVal1 + cubeVal2;
	}
}
```