in [[Object-Oriented Programming|object-oriented programming]], the open-closed principle (OCP) states "software [[Entity|entities]] ([[Class (computer programming)|classes]], modules, [[Function|functions]], etc.) should be open for extension, but closed for modification"

that is, such an entity can allow its behavior to be extended without modifying its [[Source code|source code]].

it is one of the five [[SOLID]] principles.

- a module will be said to be open if it is still available for extension. for example, it should be possible to add fields to the data structures it contains, or new elements to the set of functions it performs.
- a module will be said to be closed if [it] is available for use by other modules. this assumes that the module has been given a well-defined, stable description (the interface in the sense of information hiding)