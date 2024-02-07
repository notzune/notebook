in [[Theoretical computer science (TCS)|theoretical computer science]], an [[Algorithm|algorithm]] is correct with respect to a specification if it behaves as specified. 

an example is functional correctness, which refers to the input-output behavior of the algorithm (i.e., for each input it produces an output satisfying the specification).

partial correctness, requiring that if an answer is returned it will be correct, is distinguished from total correctness, which additionally requires that an answer is eventually returned, i.e. the algorithm terminates. 

to [[Mathematical proof|prove]] a [[Computer program|program]]'s total correctness, it is sufficient to prove its partial correctness, and its termination. 

the latter kind of proof (termination proof) can never be fully automated, since the halting problem is undecidable.