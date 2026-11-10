
# Exercise 15: Associativity of Multiplication and Different Calculation Paths

## Question

Given the matrices:

$$
A=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
$$

$$
B=
\begin{pmatrix}
1&0\\
2&1\\
-1&3
\end{pmatrix}
$$

$$
C=
\begin{pmatrix}
2&1\\
0&-1
\end{pmatrix}
$$

Compute (AB)C and A(BC). Compare the results and the number of intermediate operations. Explain what associativity of matrix multiplication means in this example.

## Solution

### 1. Identify the Dimensions of the Matrices

We are given three matrices:

- Matrix A has dimensions 2 × 3.
- Matrix B has dimensions 3 × 2.
- Matrix C has dimensions 2 × 2.

Both calculation paths are possible because the number of columns in the first matrix matches the number of rows in the second matrix.

We will calculate both expressions separately and compare their results.

### 2. Calculate the First Path: (AB)C

First, we calculate AB.

$$
AB=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
\begin{pmatrix}
1&0\\
2&1\\
-1&3
\end{pmatrix}
$$

Calculating each entry:

First row, first column:

$$
1(1)+2(2)+0(-1)=5
$$

First row, second column:

$$
1(0)+2(1)+0(3)=2
$$

Second row, first column:

$$
0(1)+1(2)+1(-1)=1
$$

Second row, second column:

$$
0(0)+1(1)+1(3)=4
$$

Therefore:

$$
AB=
\begin{pmatrix}
5&2\\
1&4
\end{pmatrix}
$$

Now, we multiply the result by matrix C:

$$
(AB)C=
\begin{pmatrix}
5&2\\
1&4
\end{pmatrix}
\begin{pmatrix}
2&1\\
0&-1
\end{pmatrix}
$$

Calculating each entry:

First row, first column:

$$
5(2)+2(0)=10
$$

First row, second column:

$$
5(1)+2(-1)=3
$$

Second row, first column:

$$
1(2)+4(0)=2
$$

Second row, second column:

$$
1(1)+4(-1)=-3
$$

Therefore:

$$
\boxed{
(AB)C=
\begin{pmatrix}
10&3\\
2&-3
\end{pmatrix}
}
$$

### 3. Calculate the Second Path: A(BC)

This time, we first calculate BC.

$$
BC=
\begin{pmatrix}
1&0\\
2&1\\
-1&3
\end{pmatrix}
\begin{pmatrix}
2&1\\
0&-1
\end{pmatrix}
$$

Calculating each entry:

First row, first column:

$$
1(2)+0(0)=2
$$

First row, second column:

$$
1(1)+0(-1)=1
$$

Second row, first column:

$$
2(2)+1(0)=4
$$

Second row, second column:

$$
2(1)+1(-1)=1
$$

Third row, first column:

$$
-1(2)+3(0)=-2
$$

Third row, second column:

$$
-1(1)+3(-1)=-4
$$

Therefore:

$$
BC=
\begin{pmatrix}
2&1\\
4&1\\
-2&-4
\end{pmatrix}
$$

Now, we multiply matrix A by the result:

$$
A(BC)=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
\begin{pmatrix}
2&1\\
4&1\\
-2&-4
\end{pmatrix}
$$

Calculating each entry:

First row, first column:

$$
1(2)+2(4)+0(-2)=10
$$

First row, second column:

$$
1(1)+2(1)+0(-4)=3
$$

Second row, first column:

$$
0(2)+1(4)+1(-2)=2
$$

Second row, second column:

$$
0(1)+1(1)+1(-4)=-3
$$

Therefore:

$$
\boxed{
A(BC)=
\begin{pmatrix}
10&3\\
2&-3
\end{pmatrix}
}
$$

### 4. Compare the Two Results

We obtained the following results:

First calculation path:

$$
(AB)C=
\begin{pmatrix}
10&3\\
2&-3
\end{pmatrix}
$$

Second calculation path:

$$
A(BC)=
\begin{pmatrix}
10&3\\
2&-3
\end{pmatrix}
$$

Both results are exactly equal.

Therefore:

$$
\boxed{(AB)C=A(BC)}
$$

This confirms that matrix multiplication is associative for these matrices.

### 5. Compare the Number of Intermediate Operations

Both calculation paths require two matrix multiplications.

However, the number of scalar arithmetic operations is different.

For the first path, (AB)C:

- Calculating AB requires 12 scalar multiplications and 8 additions.
- Multiplying AB by C requires 8 scalar multiplications and 4 additions.

Total:

$$
12+8=20 \text{ multiplications}
$$

$$
8+4=12 \text{ additions}
$$

For the second path, A(BC):

- Calculating BC requires 12 scalar multiplications and 6 additions.
- Multiplying A by BC requires 12 scalar multiplications and 8 additions.

Total:

$$
12+12=24 \text{ multiplications}
$$

$$
6+8=14 \text{ additions}
$$

Comparison:

| Calculation path | Multiplications | Additions |
|---|---:|---:|
| (AB)C | 20 | 12 |
| A(BC) | 24 | 14 |

The first calculation path requires fewer scalar operations.

Therefore, although both paths produce the same result, calculating AB first is more efficient in this example.

### 6. Explain the Associativity of Matrix Multiplication

Associativity means that changing the grouping of matrix multiplications does not change the final result.

In general:

$$
(AB)C=A(BC)
$$

This does not mean that matrices can be multiplied in any order. The order of the matrices must remain unchanged.

In our example:

- First, we multiplied A by B and then by C.
- Second, we multiplied B by C and then by A.
- Both calculation paths produced the same final matrix.

This demonstrates that matrix multiplication is associative but not necessarily commutative.

### 7. Final Conclusion

We have calculated both (AB)C and A(BC) and obtained the same result:

$$
\boxed{
(AB)C=A(BC)=
\begin{pmatrix}
10&3\\
2&-3
\end{pmatrix}
}
$$

We also observed that the first calculation path requires fewer scalar arithmetic operations than the second one.

Therefore, this exercise demonstrates two important properties of matrix multiplication:

1. Matrix multiplication is associative because changing the grouping does not change the final result.
2. The choice of calculation path can affect computational efficiency, even when the mathematical result remains the same.

Thus, associativity allows us to choose the more efficient grouping when multiplying several matrices.
