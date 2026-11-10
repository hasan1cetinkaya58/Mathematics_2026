# Exercise 4: Matrix Multiplication and Noncommutativity

## Question

For the matrices

$$
A=\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix},
\qquad
B=\begin{pmatrix}
2 & 0\\
3 & 1
\end{pmatrix}
$$

Compute:

1. $AB$
2. $BA$

Determine whether $AB=BA$ and use this example to explain the noncommutativity of matrix multiplication.

## Solution

### 1. Matrix Multiplication Rule

To multiply two matrices, we multiply each row of the first matrix by each column of the second matrix.

For two matrices to be multiplied, the number of columns of the first matrix must equal the number of rows of the second matrix.

Both $A$ and $B$ are $2\times 2$ matrices. Therefore, both products $AB$ and $BA$ are defined and have size $2\times 2$.

### 2. Calculate $AB$

We multiply matrix $A$ by matrix $B$:

$$
AB=
\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0\\
3 & 1
\end{pmatrix}
$$

Calculate each entry using row-by-column multiplication:

- First row, first column:

$$
1\cdot2+2\cdot3=2+6=8
$$

- First row, second column:

$$
1\cdot0+2\cdot1=0+2=2
$$

- Second row, first column:

$$
0\cdot2+1\cdot3=0+3=3
$$

- Second row, second column:

$$
0\cdot0+1\cdot1=0+1=1
$$

Therefore,

$$
\boxed{
AB=
\begin{pmatrix}
8 & 2\\
3 & 1
\end{pmatrix}
}
$$

### 3. Calculate $BA$

Now we reverse the order and multiply matrix $B$ by matrix $A$:

$$
BA=
\begin{pmatrix}
2 & 0\\
3 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix}
$$

Calculate each entry:

- First row, first column:

$$
2\cdot1+0\cdot0=2
$$

- First row, second column:

$$
2\cdot2+0\cdot1=4
$$

- Second row, first column:

$$
3\cdot1+1\cdot0=3
$$

- Second row, second column:

$$
3\cdot2+1\cdot1=6+1=7
$$

Therefore,

$$
\boxed{
BA=
\begin{pmatrix}
2 & 4\\
3 & 7
\end{pmatrix}
}
$$

### 4. Compare $AB$ and $BA$

We obtained:

$$
AB=
\begin{pmatrix}
8 & 2\\
3 & 1
\end{pmatrix}
$$

and

$$
BA=
\begin{pmatrix}
2 & 4\\
3 & 7
\end{pmatrix}
$$

The corresponding entries are not all equal. For example, the top-left entries are different:

$$
8\ne2
$$

Therefore,

$$
\boxed{AB\ne BA}
$$

### 5. Explanation of Noncommutativity

Noncommutativity means that changing the order of multiplication can change the result.

For ordinary real numbers, multiplication is commutative:

$$
a\cdot b=b\cdot a
$$

However, matrix multiplication is generally not commutative because the order of the matrices affects the row-by-column calculations.

This example demonstrates that multiplying $A$ by $B$ gives a different result from multiplying $B$ by $A$.

Therefore, matrix multiplication is generally noncommutative.

## Final Answers

$$
\boxed{
AB=
\begin{pmatrix}
8 & 2\\
3 & 1
\end{pmatrix}
}
$$

$$
\boxed{
BA=
\begin{pmatrix}
2 & 4\\
3 & 7
\end{pmatrix}
}
$$

$$
\boxed{AB\ne BA}
$$
