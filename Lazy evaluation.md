in [[Programming language theory (PLT)|programming language theory]], lazy evaluation, or **call-by-need**, is an [[Evaluation strategy|evaluation strategy]] which delays the evaluation of an [[Expression (computer science)|expression]] until its [[Value (computer science)|value]] is needed (non-strict evaluation) and which also avoids repeated evaluations (by the use of [[Sharing (computer science)|sharing]])

lazy evaluation is often combined with [[Memoization|memoization]]. after a function's value is computed for that [[Parameter (computer science)|parameter]] or [[Sets|set]] of parameters, the result is stored in a [[Lookup table|lookup table]] that is indexed by the values of those parameters. 

the next time the function is called, the table is consulted first to determine whether the result for that combination of parameter values is already available. if so, the stored result is simply returned; if not, the function is evaluated and another entry is added to the lookup table for reuse.

the benefits of lazy evaluation include:

- the ability to define [[Control flow|control flow]] (structures) as abstractions instead of [[Language primitive|primitives]].
- the ability to define [[Actual infinity|potentially infinite]] [[Data structure|data structures]]. this allows for more straightforward implementation of some [[Algorithm|algorithms]].
- the ability to define partly-defined data structures where some elements are errors. this allows for rapid prototyping

lazy evaluation allows control structures to be defined normally, and not as primitives or compile-time techniques. for example one can define [[Conditional (computer programming)|if-then-else]] and [[Short-circuit evaluation|short-circuit evaluation]] operators:

```haskell
ifThenElse True b c = b
ifThenElse False b c = c

-- or
True || b = True
False || b = b

-- and
True && b = b
False && b = False
```

these have the usual semantics, i.e., `ifThenElse a b c` evaluates (a), then if and only if (a) evaluates to true does it evaluate (b), otherwise it evaluates (c). that is, exactly one of (b) or (c) will be evaluated. 

similarly, for `EasilyComputed || LotsOfWork`, if the easy part gives **True** the lots of work expression could be avoided. 

finally, when evaluating `SafeToTry && Expression`, if *SafeToTry* is **false** there will be no attempt at evaluating the *Expression*.

[[Java]] doesn't support lazy evaluation natively in the same way as functional programming languages like [[Haskell]]; however, you can simulate lazy evaluation using lambda expressions which allow you to defer the execution of a piece of code until it's explicitly called.

```java
import java.util.function.Supplier;

public class LazyEvaluationExample {

    public static <T> T ifThenElse(boolean condition, Supplier<T> ifTrue, Supplier<T> ifFalse) {
        return condition ? ifTrue.get() : ifFalse.get();
    }

    public static void main(String[] args) {
        // Example of lazy if-then-else
        Supplier<String> lazyTrue = () -> "Evaluated True Branch";
        Supplier<String> lazyFalse = () -> "Evaluated False Branch";

        String result = ifThenElse(true, lazyTrue, lazyFalse);
        System.out.println(result); // Only "Evaluated True Branch" will be evaluated and printed.

        // Simulating short-circuit evaluation
        boolean a = true; // EasilyComputed
        Supplier<Boolean> lotsOfWork = () -> {
            // simulate lots of work
            return true; // the result of the work
        };

        // Lazy OR (||) - short-circuit evaluation
        boolean orResult = a || lotsOfWork.get(); // lotsOfWork will not be evaluated due to short-circuiting

        // Lazy AND (&&) - short-circuit evaluation
        boolean safeToTry = false; // SafeToTry
        Supplier<Boolean> expression = () -> true; // Expression that could throw an exception or be expensive

        boolean andResult = safeToTry && expression.get(); // expression will not be evaluated, preserving safety
    }
}
```

in this Java example, the `ifThenElse` method is a generic method that takes a boolean condition and two `Supplier` instances. 

suppliers are functional interfaces in Java that provide a single method, `get()`, which doesn't take any arguments but returns a value of a specified type. 

by using `Supplier`, we defer the execution of the `ifTrue` and `ifFalse` branches until one of them is explicitly called with `.get()`. this simulates lazy evaluation because neither the `ifTrue` nor the `ifFalse` branch is evaluated until it's absolutely necessary, based on the condition.

the example also simulates short-circuit evaluation for logical OR (`||`) and AND (`&&`) operations using boolean conditions and suppliers. the key point here is that in an eager evaluation context, both sides of the logical operation would be evaluated upfront. 

however, by using Java's built-in short-circuiting behavior for `||` and `&&` with suppliers, we can achieve a form of lazy evaluation, where the second operand is evaluated only if necessary.

this technique can be particularly useful for avoiding expensive computations that aren't needed or ensuring that potentially unsafe operations (like dereferencing null) are not performed unless certain conditions are met.