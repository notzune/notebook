in [[Computer programming|computer programming]], specifically [[Object-Oriented Programming|object-oriented programming]], a class invariant (or type invariant) is an [[Invariant|invariant]] used for constraining [[Object (computer science)|objects]] of a [[Class (computer programming)|class]]. 

[[Function (computer programming)|methods]] of the class should preserve the invariant. the class invariant constrains the state stored in the object.

class invariants are established during [[Constructor (computer programming)|construction]] and constantly maintained between calls to public methods. code within functions may break invariants as long as the invariants are restored before a public function ends.

with [[Concurrent computing|concurrency]], maintaining the invariant in methods typically requires a critical section to be established by locking the state using a [[Lock (computer science)|mutex]].