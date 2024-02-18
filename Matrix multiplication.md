[[Matrices|matrix]] multiplication is a fundamental [[Operation|operation]] in [[Linear algebra|linear algebra]] and [[Discrete mathematics|discrete mathematics]] and is used in fields like [[Computer science|computer science]], specifically in fields like [[Computer graphics|graphic engineering]] and [[Machine learning|machine learning]].

the basic idea behind matrix multiplication is that you can multiply two matrices, $A$ and $B$, to get a new matrix $C$.

for the multiplication to be valid, the number of columns in $A$ must match the number of rows in $B$. 

if $A$ is an $m\times n$ matrix and $B$ is an $n\times p$ matrix, the resulting $C$ matrix will be an $m\times p$ matrix

the entry in the $i$-th row and $j$-th column of matrix $C$, denoted as $C_{ij}$, is [[Computation|computed]] as the [[Dot product|dot product]] of the $i$-th row of matrix $A$ and the $j$-th column of matrix $B$.

$$
C_{ij}=\sum^{n}_{k=1}A_{ik}\,B_{kj}
$$

# Implementation

the simplest [[Algorithm|algorithm]] for matrix multiplication is the naive approach, which directly implements the above definition. here is an example written in [[Java]]

```java
public class MatrixMultiplication {

    /**
     * Multiplies two matrices and returns the result.
     * @param A The first matrix (m x n).
     * @param B The second matrix (n x p).
     * @return The product matrix (m x p).
     */
    public static int[][] multiplyMatrices(int[][] A, int[][] B) {
        int m = A.length; // # of rows in A.
        int n = A[0].length; // # of columns in A (rows in B).
        int p = B[0].length; // # of columns in B.
        
        // Result
        int[][] C = new int[m][p];

        // Compute each element of the product matrix.
        for (int i = 0; i < m; i++) {
            for (int j = 0; j < p; j++) {
                for (int k = 0; k < n; k++) {
                    C[i][j] += A[i][k] * B[k][j];
                }
            }
        }

        return C;
    }

    public static void main(String[] args) {
        // Example matrices A and B.
        int[][] A = {{1, 2}, {3, 4}};
        int[][] B = {{5, 6}, {7, 8}};
        
        // Multiply matrices A and B.
        int[][] C = multiplyMatrices(A, B);

        // Print the result matrix C.
        System.out.println("Product of A and B is:");
        for (int[] row : C) {
            for (int value : row) {
                System.out.print(value + " ");
            }
            System.out.println();
        }
    }
}
```

## [[Time complexity]]

the time complexity of this (in [[Big O notation (O)|big O notation]]) is $O(mnp)$, where $m$ is the number of rows in the first matrix, $n$ is the number of columns in the first matrix (and the number of rows of the second), and $p$ is the number of columns in the second matrix.

this is because for each of the $mp$ entries of the resulting matrix, we perform $n$ multiplications and $n-1$ additions (which can be considered constant time operations)