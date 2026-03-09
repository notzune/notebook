in [[Computer programming|computer programming]], the return type (or result type) defines the constrains the [[Data type|data type]] of the value [[Return statement|returned]] from a subroutine or [[Function (computer programming)|method]]. in many [[Programming language|programming languages]] (especially [[Type system|statically-typed programming languages]] such as [[Java]]), the return type must be explicitly specified when declaring a function.

```java
public void setSum(int n1, int n2) {
    sum = n1 + n2
}

public int getSum() {
    return sum;
}
```

the return type is [[Integer (computer science)|int]]. the program can therefore rely on the method returning a value of type int. 

for the case where a subroutine does not return any value, e.g., a return type of [[Void type|void]] is used in some programming languages:

```java
public void returnNothing()
```