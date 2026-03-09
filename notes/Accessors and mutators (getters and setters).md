because [[Instance variable|instance data]] is usually set to [[Access modifier|private]], a [[Class (computer programming)|class]] usually provides services to access and modify those data values.

an ***accessor*** [[Function (computer programming)|method]] returns the [[State (computer science)|current]] value of a [[Variable (computer science)|variable]], while a ***mutator*** method changes the value of a variable.

the names of accessor and mutator methods take the form of `getFoo` and `setFoo`, respectively (where `Foo` is just a [[Foobar|placeholder]]); these methods are also commonly referred to as "getters" and "setters".

the use of mutators gives the programmer the ability to restrict a client's options to modify an object's state. often the mutator is designed so that the values of variables can be set only within particular limits.