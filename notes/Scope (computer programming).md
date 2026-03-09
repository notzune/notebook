the scope of a [[Name binding|name binding]] an association of a name to an entity, such as a [[Variable (computer science)|variable]]) is the part of a [[Computer program|program]] where that name binding is valid; in other words, where the name can be used to refer to the entity.

in other parts of the program, the name may refer to a different entity (it may have a different binding), or to nothing at all (it may be unbound). 

scope helps prevent [[Name collision|name collisions]] by allowing the same name to refer to different objects – as long as the names have separate scopes.

- data declared at the [[Class (computer programming)|class]] level can be referenced by all [[Function (computer programming)|methods]] in that class; this is also referred to as [[Instance variable|instance data]].
- data declared within a method can be used only in that method
- data declared within a method is called local data