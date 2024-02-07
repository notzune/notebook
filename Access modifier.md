access modifiers are [[Reserved word|keywords]] in [[Object-Oriented Programming|object-oriented languages]] that set the accessibility of [[Class (computer programming)|classes]], [[Function composition (computer science)|methods]], and other members. they are used to facilitate the [[Encapsulation (computer programming)|encapsulation]] of components.

access modifiers change the [[Scope (computer programming)|scope]] of whatever data they are modifying.

in [[Java]], there are four access modifiers:

| Name of Modifier | Scope |
| ---- | ---- |
| `private` | class |
| `protected` | derived classes and/or within same [[Package (object-oriented programming)\|package]]. |
| `package` | within its package |
| `public` | everybody |

members of a class that are declared with `public` can be referenced anywhere, while `private` can only be referenced within that class.

members declared without a visibility stated explicitly will have an implicit "default" access and can be referenced by any class in the same package.

public access modifiers violate encapsulation because they allow the client to modify the values directly, therefore instance variables should not be declared with public visibility. 

it is acceptable to give a constant public visibility which allows it to be used outside of the class.

public constants do not violate encapsulation because, although the client can access it, its value cannot be changed.