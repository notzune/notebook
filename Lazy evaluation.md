in [[Programming language theory (PLT)|programming language theory]], lazy evaluation, or **call-by-need**, is an [[Evaluation strategy|evaluation strategy]] which delays the evaluation of an [[Expression (computer science)|expression]] until its [[Value (computer science)|value]] is needed (non-strict evaluation) and which also avoids repeated evaluations (by the use of [[Sharing (computer science)|sharing]])

lazy evaluation is often combined with [[Memoization|memoization]]. after a function's value is computed for that [[Parameter (computer science)|parameter]] or [[Sets|set]] of parameters, the result is stored in a [[Lookup table|lookup table]] that is indexed by the values of those parameters. 

the next time the function is called, the table is consulted first to determine whether the result for that combination of parameter values is already available. if so, the stored result is simply returned; if not, the function is evaluated and another entry is added to the lookup table for reuse.

the benefits of lazy evaluation include:

- the ability to define [[Control flow|control flow]] (structures) as abstractions instead of [[Language primitive|primitives]].