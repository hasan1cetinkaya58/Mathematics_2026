# Exercise 12. A Parameter Revealed by a Row Operation

## Question

For the matrix

$$
A(t)=
\begin{pmatrix}
1 & 2 & 3\\
2 & 4 & t\\
0 & 1 & 1
\end{pmatrix}
$$

find the values of $t$ for which the matrix is not invertible.

Before computing the determinant, perform the operation

$$
R_2 \leftarrow R_2-2R_1
$$

and use the resulting structure. At the end, explain what special thing happens to the rows for the value of the parameter you found.

> **Why this exercise:** combines a parameter, row operations, and recognition of dependence in one short argument.

## Solution

### Step 1. Apply the Prescribed Row Operation

We are given:

$$
A(t)=
\begin{pmatrix}
1 & 2 & 3\\
2 & 4 & t\\
0 & 1 & 1
\end{pmatrix}
$$

First, perform the required row operation:

$$
R_2 \leftarrow R_2-2R_1
$$

The new second row is:

$$
(2,4,t)-2(1,2,3)
$$

$$
=(2-2,\;4-4,\;t-6)
$$

$$
=(0,0,t-6)
$$

Therefore, the resulting matrix is:

$$
\begin{pmatrix}
1 & 2 & 3\\
0 & 0 & t-6\\
0 & 1 & 1
\end{pmatrix}
$$

### Step 2. Calculate the Determinant

Adding a multiple of one row to another row does not change the determinant.

Therefore, the determinant of the resulting matrix is equal to the determinant of the original matrix.

Expanding along the second row gives:

$$
\det(A(t))
=-(t-6)
\begin{vmatrix}
1 & 2\\
0 & 1
\end{vmatrix}
$$

The remaining determinant is:

$$
\begin{vmatrix}
1 & 2\\
0 & 1
\end{vmatrix}
=1\cdot1-2\cdot0=1
$$

Thus:

$$
\det(A(t))=-(t-6)=6-t
$$

### Step 3. Find the Value for Which the Matrix Is Not Invertible

A square matrix is not invertible if and only if its determinant is zero.

Set the determinant equal to zero:

$$
6-t=0
$$

Therefore:

$$
\boxed{t=6}
$$

### Step 4. Explain What Happens to the Rows

For $t=6$, the resulting matrix becomes:

$$
\begin{pmatrix}
1 & 2 & 3\\
0 & 0 & 0\\
0 & 1 & 1
\end{pmatrix}
$$

The second row becomes a zero row.

In the original matrix, when $t=6$, the second row is:

$$
R_2=(2,4,6)
$$

while the first row is:

$$
R_1=(1,2,3)
$$

Therefore:

$$
R_2=2R_1
$$

This means that the second row is a multiple of the first row. The rows are linearly dependent, so the matrix does not have full rank and is not invertible.

### Step 5. Final Answer

$$
\boxed{t=6}
$$

**Conclusion:** The matrix is not invertible only when $t=6$. At this value, the second row of the original matrix is twice the first row. After applying the prescribed row operation, the second row becomes a zero row, clearly showing the linear dependence of the rows.
