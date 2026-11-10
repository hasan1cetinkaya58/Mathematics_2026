
# Exercise 6: Transpose

## Question

For the matrices

$$
A=
\begin{pmatrix}
1&2&3\\
4&5&6
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
1&0\\
2&1\\
-1&3
\end{pmatrix}
$$

Compute $A^T$, $B^T$, and $AB$.

Then verify in this example that

$$
(AB)^T=B^TA^T.
$$

## Solution

### 1. Understanding Matrix Transposition

The transpose of a matrix is obtained by changing its rows into columns and its columns into rows.

In other words, the element in row $i$ and column $j$ becomes the element in row $j$ and column $i$.

If a matrix has dimensions $m\times n$, its transpose has dimensions $n\times m$.

The given matrices are:

$$
A=
\begin{pmatrix}
1&2&3\\
4&5&6
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

Matrix $A$ has dimensions $2\times3$, and matrix $B$ has dimensions $3\times2$.

### 2. Calculate the Transpose of Matrix A

To calculate $A^T$, we convert the rows of $A$ into columns.

The first row of $A$, $(1,2,3)$, becomes the first column of $A^T$.

The second row of $A$, $(4,5,6)$, becomes the second column of $A^T$.

Therefore,

$$
A^T=
\begin{pmatrix}
1&4\\
2&5\\
3&6
\end{pmatrix}
$$

The original matrix has dimensions $2\times3$, so its transpose has dimensions $3\times2$.

### 3. Calculate the Transpose of Matrix B

We apply the same rule to matrix $B$.

The rows of $B$ become the columns of $B^T$.

The first row $(1,0)$ becomes the first column.

The second row $(2,1)$ becomes the second column.

The third row $(-1,3)$ becomes the third column.

Therefore,

$$
B^T=
\begin{pmatrix}
1&2&-1\\
0&1&3
\end{pmatrix}
$$

The original matrix has dimensions $3\times2$, so its transpose has dimensions $2\times3$.

### 4. Calculate the Matrix Product AB

First, we check whether the multiplication is defined.

Matrix $A$ has dimensions $2\times3$, and matrix $B$ has dimensions $3\times2$.

The number of columns of $A$ is equal to the number of rows of $B$.

Since $3=3$, the multiplication is defined.

The resulting matrix has dimensions $2\times2$.

Now we calculate the product using row-by-column multiplication.

$$
AB=
\begin{pmatrix}
1&2&3\\
4&5&6
\end{pmatrix}
\begin{pmatrix}
1&0\\
2&1\\
-1&3
\end{pmatrix}
$$

**First row, first column:**

$$
1\cdot1+2\cdot2+3\cdot(-1)
=1+4-3=2
$$

**First row, second column:**

$$
1\cdot0+2\cdot1+3\cdot3
=0+2+9=11
$$

**Second row, first column:**

$$
4\cdot1+5\cdot2+6\cdot(-1)
=4+10-6=8
$$

**Second row, second column:**

$$
4\cdot0+5\cdot1+6\cdot3
=0+5+18=23
$$

Combining all four calculated entries, we obtain:

$$
\boxed{
AB=
\begin{pmatrix}
2&11\\
8&23
\end{pmatrix}
}
$$

### 5. Calculate the Transpose of AB

We already calculated:

$$
AB=
\begin{pmatrix}
2&11\\
8&23
\end{pmatrix}
$$

To calculate $(AB)^T$, we exchange the rows and columns.

The first row $(2,11)$ becomes the first column.

The second row $(8,23)$ becomes the second column.

Therefore,

$$
\boxed{
(AB)^T=
\begin{pmatrix}
2&8\\
11&23
\end{pmatrix}
}
$$

### 6. Calculate the Product B^T A^T

Now we calculate the right-hand side of the required identity.

We already obtained:

$$
B^T=
\begin{pmatrix}
1&2&-1\\
0&1&3
\end{pmatrix}
$$

and

$$
A^T=
\begin{pmatrix}
1&4\\
2&5\\
3&6
\end{pmatrix}
$$

Therefore,

$$
B^TA^T=
\begin{pmatrix}
1&2&-1\\
0&1&3
\end{pmatrix}
\begin{pmatrix}
1&4\\
2&5\\
3&6
\end{pmatrix}
$$

Both matrices can be multiplied because their inner dimensions are equal: $3=3$.

The resulting matrix has dimensions $2\times2$.

**First row, first column:**

$$
1\cdot1+2\cdot2+(-1)\cdot3
=1+4-3=2
$$

**First row, second column:**

$$
1\cdot4+2\cdot5+(-1)\cdot6
=4+10-6=8
$$

**Second row, first column:**

$$
0\cdot1+1\cdot2+3\cdot3
=0+2+9=11
$$

**Second row, second column:**

$$
0\cdot4+1\cdot5+3\cdot6
=0+5+18=23
$$

Thus,

$$
\boxed{
B^TA^T=
\begin{pmatrix}
2&8\\
11&23
\end{pmatrix}
}
$$

### 7. Verify the Transpose Property

The property we need to verify is:

$$
(AB)^T=B^TA^T
$$

From the previous calculations, we obtained:

$$
(AB)^T=
\begin{pmatrix}
2&8\\
11&23
\end{pmatrix}
$$

and

$$
B^TA^T=
\begin{pmatrix}
2&8\\
11&23
\end{pmatrix}
$$

Both sides produce exactly the same matrix.

Therefore,

$$
\boxed{(AB)^T=B^TA^T}
$$

The identity is verified for the given matrices.

### 8. Explanation of the Transpose Property

This example demonstrates an important property of matrix transposition.

The transpose of a product of two matrices equals the product of their transposes in reverse order.

In general:

$$
(AB)^T=B^TA^T
$$

The order of the matrices must be reversed when taking the transpose of a product.

This means that we cannot simply write $A^TB^T$.

The correct order is $B^TA^T$.

## Final Answer

The transpose of matrix A is:

$$
\boxed{
A^T=
\begin{pmatrix}
1&4\\
2&5\\
3&6
\end{pmatrix}
}
$$

The transpose of matrix B is:

$$
\boxed{
B^T=
\begin{pmatrix}
1&2&-1\\
0&1&3
\end{pmatrix}
}
$$

The matrix product is:

$$
\boxed{
AB=
\begin{pmatrix}
2&11\\
8&23
\end{pmatrix}
}
$$

The transpose identity is verified:

$$
\boxed{
(AB)^T=B^TA^T=
\begin{pmatrix}
2&8\\
11&23
\end{pmatrix}
}
$$

**Conclusion:** The calculations confirm that the transpose of a matrix product equals the product of the transposed matrices in reverse order.
