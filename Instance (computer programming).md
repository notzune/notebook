in [[Object-Oriented Programming|object-oriented programming]], an instance is a concrete occurrence of any [[Object (computer science)|object]], existing usually during the runtime of a computer program.

in java, using the `new` operator will create a new instance of an object class.

for example, we can [[Declaration (computer science)|declare]] an object ([[Foobar|foobar]]) as a variable

```java
// here we are declaring a variable

Object foo;
```

and then instantiate (create a new instance of) it.

```java 
// and here we are instantiating it

foo = new Object(bar);
```

in typical case, the process is as follows:

- calculate the size of an object – the size is mostly the same as that of the [[Class (computer programming)|class]] but can vary. when the object in question is not derived from a class, but from a [[Prototype based programming|prototype]] instead, the size of an object is usually that of the internal data structure (a hash for instance) that holds its slots.
- allocation – allocating memory space with the size of an object plus the growth later, if possible to know in advance
- [[Name binding|binding]] methods – this is usually either left to the class of the object, or is resolved at dispatch, but nevertheless it is possible that some object models bind methods at creation time.
- calling an initializing code (namely, [[Constructor (computer programming)|constructor]]) of [[Superclass (computer programming)|superclass]]
- calling an initializing code of class being created