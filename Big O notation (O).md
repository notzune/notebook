big O notation is a mathematical notation that describes the [[Limit|limiting]] behavior of a [[Function|function]] when the [[Argument of a function|argument]] tends towards a particular value or infinity. 

big O is a member of the [[Family of notations|family of notations]] collectively called asymptotic notation.

in [[Computer science|computer science]], big O notation is used to [[Computational complexity theory|classify]] [[Algorithm|algorithms]] according to how their run time or space requirements grow as the input size grows.

a description of a function in terms of big O notation usually only provides an [[Upper and lower bounds|upper bound]] on the growth rate of the [[Function (computer programming)|function]].

# Example

consider this simple [[Algorithm|algorithm]] (written in [[Psuedocode|psuedocode]]) that finds the maximum [[Element|element]] in an  unsorted [[Array (datatype)|array]]

```
function findMax(array):
    maxElement = array[0]
    for each element in array:
        if element > maxElement:
            maxElement = element
    return maxElement
```

in this algorithm, we iterate through each element of the array once to find the maximum value.

the time it takes to complete this operation is directly proportional to the number of elements in the array. if the array has $n$ elements, the algorithm performs $n$ comparisons. 

in big O notation, this [[Time complexity|time complexity]] is expressed as $O(n)$. this notation tells us that the maximum number of operations (in this case, comparisons) needs to grow [[Linear|linearly]] with the size of the input. it provides an upper bound on the growth rate, indicating that the algorithm will not perform worse than [[Linear time|linear time]] in relation to the size of the input.