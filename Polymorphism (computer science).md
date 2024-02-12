in [[Programming language theory (PLT)|programming language theory]] and [[Type theory|type theory]], polymorphism is the use of a single symbol to represent multiple different types.

in [[Object-Oriented Programming|OOP]], polymorphism is the provision of a single [[Interface (computer science)|interface]] to entities of different [[Data type|types]]. the concept is borrowed from a principle in biology where an [[Organism|organism]] or [[Species|species]] can have many different forms or stages.

the most commonly used forms of polymorphism are:

- [[Ad hoc polymorphism|ad hoc polymorphism]] -  defines a common interface for an arbitrary set of individually specified types
- [[Parametric polymorphism|parametric polymorphism]] - not specifying [[Concrete implementation|concrete]] types and instead use [[Abstract data type|abstract]] symbols that can substitute for any type
- [[Subtyping|subtyping]] - (also called inclusion polymorphism): when a name denotes instances of many different classes related by some common [[Superclass (computer programming)|superclass]].

# [[Ad hoc polymorphism]]

refers to polymorphic functions that can be applied to arguments of different types, but that behave differently depending on the type of the argument to which they are applied (also known as [[Function overloading|function overloading]] or [[Operator overloading|operator overloading]])

in this [[Java]] example, the `Add` [[Function (computer programming)|function]] seems to work generically over two types ([[Integer (data type)|integer]] and [[String (data type)|string]]) but are considered to be two entirely different functions by the [[Compiler|compiler]].

```java
class AdHocPolymorphic {
    public String add(int x, int y) {
        return "Sum: "+(x+y);
    }

    public String add(String name) {
        return "Added "+name;
    }
}

public class adhoc {
    public static void main(String[] args) {
        AdHocPolymorphic poly = new AdHocPolymorphic();

        System.out.println( poly.add(1,2)   ); // prints "Sum: 3"
        System.out.println( poly.add("Zune") ); // prints "Added Zune"
    }
}
```

# [[Parametric polymorphism]]

allows a function or a data type to be written generically, so that it can handle values uniformly without depending on their type. this means that the same piece of code can operate on various data types, making your programs more flexible and reusable.

the most common implementation of parametric polymorphism in Java is through the use of the [[Generic type|generic type]], `T`, such as in this example:

```java
class GenericAdd<T> {
    public T add(T a, T b) {
	    // here we add logic to support the specific data type, without having to create multiple methods for each
        if (a instanceof Integer && b instanceof Integer) {
            return (T) Integer.valueOf(((Integer) a) + ((Integer) b));
        } else if (a instanceof String && b instanceof String) {
            return (T) (a.toString() + b.toString());
        }
        throw new IllegalArgumentException("Unsupported types");
    }
}

public class Parametric {
    public static void main(String[] args) {
        GenericAdd<Integer> intAdder = new GenericAdd<>();
        System.out.println("Sum: " + intAdder.add(1, 2)); // prints "Sum: 3"

        GenericAdd<String> stringAdder = new GenericAdd<>();
        System.out.println("Concatenation: " + stringAdder.add("Hello, ", "zune!")); // prints "Concatenation: Hello, zune!"
    }
}
```

in this example, the `GenericAdd` class uses a type parameter `T` to operate generically on two inputs of the same type. the `add` method then checks the type of `T` at runtime to decide how to process the inputs. 

this example illustrates how parametric polymorphism can be used to write flexible and reusable code, but also highlights the need for runtime type checks when dealing with operations specific to certain types.

# [[Subtyping]]

subtyping, or inclusion polymorphism, is another form of polymorphism where a subtype can be used in places where a parent type is expected. this allows for more flexible and extensible code designs. in Java, subtyping is achieved through [[Inheritance (object-oriented programming)|inheritance]] and interface implementation.

```java
interface Addable {
    String add();
}

class IntegerAdd implements Addable {
    int x, y;

    IntegerAdd(int x, int y) {
        this.x = x;
        this.y = y;
    }

    @Override
    public String add() {
        return "Sum: " + (x + y);
    }
}

class StringAdd implements Addable {
    String a, b;

    StringAdd(String a, String b) {
        this.a = a;
        this.b = b;
    }

    @Override
    public String add() {
        return "Concatenation: " + a + b;
    }
}

public class Subtyping {
    public static void main(String[] args) {
        Addable intAdd = new IntegerAdd(1, 2);
        Addable strAdd = new StringAdd("Hello, ", "world!");

        System.out.println(intAdd.add()); // prints "Sum: 3"
        System.out.println(strAdd.add()); // prints "Concatenation: Hello, world!"
    }
}
```

in this example, `Addable` is an interface that defines an `add` method. `IntegerAdd` and `StringAdd` are two different implementations of the `Addable` interface, handling integer addition and string concatenation, respectively. 

this demonstrates how subtyping allows different types (`IntegerAdd` and `StringAdd`) to be used interchangeably through a common interface (`Addable`), showcasing the power of inclusion polymorphism in designing flexible and extensible systems.

there are more complex examples of subtyping and [[Method overriding|method overriding]]. this example features a base class with several methods, a subclass that inherits from the base class and overrides one of its methods, and another method that is unique to the subclass. 

the subclass will showcase the use of both inherited methods that it does not override and its unique method, thus demonstrating how a single instantiated class can utilize methods from its parent class along with its methods.

```java
class Vehicle {
    // A method common to all vehicles
    public void start() {
        System.out.println("Vehicle started");
    }

    // A method that can be overridden by subclasses
    public void move() {
        System.out.println("Vehicle is moving");
    }

    // A method that is not overridden by the subclass
    public void stop() {
        System.out.println("Vehicle stopped");
    }
}

class Car extends Vehicle {
    // Override the move method to provide specific implementation for Car
    @Override
    public void move() {
        System.out.println("Car is moving efficiently on the road");
    }

    // A method specific to Car
    public void playMusic() {
        System.out.println("Playing music in the car");
    }
}

public class InheritanceExample {
    public static void main(String[] args) {
        Car myCar = new Car();

        // Using the start method inherited from Vehicle
        myCar.start(); // Output: Vehicle started

        // Using the overridden move method from Car
        myCar.move(); // Output: Car is moving efficiently on the road

        // Using the stop method inherited from Vehicle, which is not overridden in Car
        myCar.stop(); // Output: Vehicle stopped

        // Using the method unique to Car
        myCar.playMusic(); // Output: Playing music in the car
    }
}
```

in this example, `Vehicle` is the parent class with three methods: `start()`, `move()`, and `stop()`. 

the `Car` class extends `Vehicle`, overriding the `move()` method to provide behavior specific to cars, and introduces a new method, `playMusic()`, which is specific to the `Car` class.

when an [[Instance (computer programming)|instance]] of `Car` is created and its methods are called:

- the `start()` and `stop()` methods are inherited from `Vehicle` and are not overridden, so they retain their original behavior.
- the `move()` method is overridden in `Car` to provide a car-specific implementation.
- the `playMusic()` method is unique to `Car` and showcases additional functionality that is not present in the parent class.