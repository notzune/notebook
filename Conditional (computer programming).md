in [[Computer science|computer science]], conditional statements are commands in a [[Programming language|programming language]] to handle decision making [[Logic (computer programming)|logic]]; they are a type of [[Conditional statement|logical conditional]].

specifically, conditionals perform different [[Computation|computations]] based on whether the [[Boolean|boolean]] statement evaluates to a true or false value.

conditionals are used heavily in [[Control flow|control flow]] design to alter the control flow based on some condition (this doesn't apply to the case of [[Predication (computer architecture)|branch prediction]]).

the `if–then` construct (sometimes called `if–then–else`) is common across many programming languages. although the syntax varies from language to language, the basic structure (in [[Psuedocode|pseudocode]] form) looks like this:

```
If (boolean condition) Then
   (consequent)
Else
   (alternative)
End if
```

for example:

```
If stock=0 Then
	message= order new stock
Else
	message= there is stock
End if
```

in [[Python]] this would look something like:

```python
# Assume stock is a variable representing the quantity of stock available
stock = 0

if stock == 0:
    message = "Order new stock"
else:
    message = "There is stock"

print(message)
```

and in [[Java]]:

```java
public class StockChecker {
    public static void main(String[] args) {
        // Assume stock is a variable representing the quantity of stock available
        int stock = 0;
        String message;

        if (stock == 0) {
            message = "Order new stock";
        } else {
            message = "There is stock";
        }

        System.out.println(message);
    }
}
```