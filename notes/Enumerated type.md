in [[Computer programming|programming]], an enumerated type (also referred to as an enum, or a [[Categorical variable|categorical variable]] in [[Statistics|statistics]]) is a [[Data type|data type]]  consisting of a [[Sets|set]] of named [[Value (computer science)|values]] called *[[Element|elements]]*, *members*, or *enumerators*. mathematically, they behave in a similar way as an [[Enumeration|enumerated set]].

the enumerator names are usually [[Identifier (computer languages)|identifiers]] that behave as [[Constant (computer programming)|constants]] in the [[Programming language|language]]. 

# Example

for example, the four suits in a [[Deck of cards|deck of cards]] may be four enumerators named `CLUB, DIAMOND, HEART` and `SPADE`, belonging to an `enum` named "Suit" (for example):

```java
public class EnumExample {
    // Define the Suit enum
    enum Suit {
        CLUB, DIAMOND, HEART, SPADE
    }

    public static void main(String[] args) {
        // Use the Suit enum
        Suit mySuit = Suit.HEART;

        // Check the value of mySuit
        switch (mySuit) {
            case CLUB:
                System.out.println("Club");
                break;
            case DIAMOND:
                System.out.println("Diamond");
                break;
            case HEART:
                System.out.println("Heart");
                break;
            case SPADE:
                System.out.println("Spade");
                break;
        }
    }
}
```

in this example, `Suit` is an `enum` that contains four constants (`CLUB`, `DIAMOND`, `HEART`, `SPADE`) representing the four suits in a deck of cards. in the `main` method, we create a variable `mySuit` of type `Suit` and assign it the value `Suit.HEART`. then, we use a `switch` statement to check the value of `mySuit` and print out the name of the suit.

enums in [[Java]] are more powerful than simple sets of constants; they can also have fields, methods, and constructors, which allows them to behave like more complex types. here's a more advanced example that demonstrates this:

```java
public class EnhancedEnumExample {
    // Define the Suit enum with a constructor and a private field
    enum Suit {
        CLUB("black"),
        DIAMOND("red"),
        HEART("red"),
        SPADE("black");

        private final String color;

        // Constructor for the enum
        Suit(String color) {
            this.color = color;
        }

        public String getColor() {
            return color;
        }
    }

    public static void main(String[] args) {
        // Iterate over all Suits and print their colors
        for (Suit suit : Suit.values()) {
            System.out.println(suit + " is " + suit.getColor());
        }
    }
}
```

in this example, each `Suit` enum now also includes a color attribute (`"black"` or `"red"`), demonstrating how enums in Java can encapsulate both data and behavior.