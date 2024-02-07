a constructor (**ctor**) is a special type of [[Function (computer programming)|method]] that gets called to [[Instance (computer programming)|create an object]]. it prepares the new object for use, often accepting [[Parameter (computer science)|arguments]] that the constructor uses to set required [[Member variable|member variables]].

it has no explicit [[Return type|return type]] and is not implicitly [[Inheritance (object-oriented programming)|inherited]] by other classes.

constructors often have the same name as the declaring [[Class (computer programming)|class]]. they have the task of [[Initialization (computer programming)|initializing]] the object's [[Field (computer science)|data members]] and of establishing the [[Class invariant|invariant of the class]].

[[Immutable object|immutable objects]] must be initialized in a constructor.

most [[Programming language|languages]] allow [[Function overloading|overloading]] the constructor in that there can be more than one constructor for a class, with differing parameters.

constructors, which concretely use a single class to create objects and return a new instance of the class, are abstracted by [[Factory (object-oriented programming)|factories]], which also create objects but can do so in various ways, using multiple classes or different allocation schemes such as an [[Object pool pattern|object pool]].