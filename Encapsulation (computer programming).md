an encapsulated [[Object (computer science)|object]] can be thought of as a [[Black box|black box]]–its inner workings are hidden from the client.  the client can then invoke the [[Interface (computer science)|interface]] methods and they manage the [[Instance (computer programming)|instance]] data.

basically, encapsulation prevents external code from being concerned with the internal workings of an object

encapsulation allows developers to present a consistent interface that is independent of its internal implementation. 

for example, encapsulation can be used to hide the values or state of a structured data object inside a [[Class (computer programming)|class]], preventing direct access to them by clients in a way that could expose hidden implementation details or violate [[State (computer science)|state]] [[Class invariant|invariance]] maintained by the methods.

it also encourages programmers to put all the code that is concerned with a certain set of data in the same class, which organizes it for easy comprehension by other programmers. 

encapsulation is a technique that encourages [[Coupling (computer programming)|decoupling]].

```java
public class Employee {

	// here we encapsulate the salary
    private BigDecimal salary = new BigDecimal(50000.00);
    
    public BigDecimal getSalary() {
        return this.salary;
    }

    public static void main() {
        Employee e = new Employee();
        BigDecimal sal = e.getSalary();
    }
}
```