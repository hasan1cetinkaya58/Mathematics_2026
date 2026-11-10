# Exercise 10: Columns of a Matrix Product

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
1&2\\
-1&0\\
3&1
\end{pmatrix}
$$

Denote the columns of $B$ by $b_1$ and $b_2$.

1. Compute $Ab_1$ and $Ab_2$.
2. Compute the matrix $AB$.
3. Compare the results and explain why the columns of $AB$ are exactly the vectors $Ab_1$ and $Ab_2$.

## Solution

### 1. Identify the Matrix Dimensions and Columns

First, we identify the dimensions of the given matrices.

Matrix $A$ has dimensions $2\times3$, and matrix $B$ has dimensions $3\times2$.

Since the number of columns of $A$ equals the number of rows of $B$, the product $AB$ is defined.

The resulting matrix will have dimensions $2\times2$.

The matrix $B$ is:

$$
B=
\begin{pmatrix}
1&2\\
-1&0\\
3&1
\end{pmatrix}
$$

Its first column is:

$$
b_1=
\begin{pmatrix}
1\\
-1\\
3
\end{pmatrix}
$$

Its second column is:

$$
b_2=
\begin{pmatrix}
2\\
0\\
1
\end{pmatrix}
$$

### 2. Calculate $Ab_1$

We multiply matrix $A$ by the first column of matrix $B$.

$$
Ab_1=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
\begin{pmatrix}
1\\
-1\\
3
\end{pmatrix}
$$

Using row-by-column multiplication:

First component:

$$
1\cdot1+2\cdot(-1)+0\cdot3
$$

$$
=1-2+0=-1
$$

Second component:

$$
0\cdot1+1\cdot(-1)+1\cdot3
$$

$$
=0-1+3=2
$$

Therefore, the result is:

$$
\boxed{
Ab_1=
\begin{pmatrix}
-1\\
2
\end{pmatrix}
}
$$

### 3. Calculate $Ab_2$

Now we multiply matrix $A$ by the second column of matrix $B$.

$$
Ab_2=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
\begin{pmatrix}
2\\
0\\
1
\end{pmatrix}
$$

Using row-by-column multiplication:

First component:

$$
1\cdot2+2\cdot0+0\cdot1
$$

$$
=2+0+0=2
$$

Second component:

$$
0\cdot2+1\cdot0+1\cdot1
$$

$$
=0+0+1=1
$$

Therefore, the result is:

$$
\boxed{
Ab_2=
\begin{pmatrix}
2\\
1
\end{pmatrix}
}
$$

### 4. Calculate the Matrix Product $AB$

Now we calculate the complete matrix product.

$$
AB=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
\begin{pmatrix}
1&2\\
-1&0\\
3&1
\end{pmatrix}
$$

We calculate each entry using row-by-column multiplication.

First row, first column:

$$
1\cdot1+2\cdot(-1)+0\cdot3=-1
$$

First row, second column:

$$
1\cdot2+2\cdot0+0\cdot1=2
$$

Second row, first column:

$$
0\cdot1+1\cdot(-1)+1\cdot3=2
$$

Second row, second column:

$$
0\cdot2+1\cdot0+1\cdot1=1
$$

Combining these four entries gives:

$$
\boxed{
AB=
\begin{pmatrix}
-1&2\\
2&1
\end{pmatrix}
}
$$

### 5. Compare the Results

We previously calculated:

$$
Ab_1=
\begin{pmatrix}
-1\\
2
\end{pmatrix}
$$

and

$$
Ab_2=
\begin{pmatrix}
2\\
1
\end{pmatrix}
$$

The complete matrix product is:

$$
AB=
\begin{pmatrix}
-1&2\\
2&1
\end{pmatrix}
$$

Notice that the first column of $AB$ is exactly $Ab_1$, and the second column of $AB$ is exactly $Ab_2$.

Therefore:

$$
\boxed{
AB=
\begin{pmatrix}
|&|\\
Ab_1&Ab_2\\
|&|
\end{pmatrix}
}
$$

### 6. Explain Why the Columns of $AB$ Are $Ab_1$ and $Ab_2$

Matrix multiplication can be understood column by column.

When we multiply matrix $A$ by matrix $B$, each column of $B$ is multiplied by $A$ separately.

The first column of $AB$ is obtained by calculating $Ab_1$.

The second column of $AB$ is obtained by calculating $Ab_2$.

This happens because matrix multiplication applies the same linear transformation represented by $A$ to every column of $B$.

Therefore, the columns of the product matrix are exactly the transformed columns of the original matrix $B$.

## Final Answer

The first column calculation is:

$$
\boxed{
Ab_1=
\begin{pmatrix}
-1\\
2
\end{pmatrix}
}
$$

The second column calculation is:

$$
\boxed{
Ab_2=
\begin{pmatrix}
2\\
1
\end{pmatrix}
}
$$

The complete matrix product is:

$$
\boxed{
AB=
\begin{pmatrix}
-1&2\\
2&1
\end{pmatrix}
}
$$

**Conclusion:**

The columns of $AB$ are exactly $Ab_1$ and $Ab_2$ because matrix multiplication applies the transformation represented by $A$ to each column of $B$ independently.

This demonstrates the relationship between matrix-vector multiplication and matrix-matrix multiplication.
