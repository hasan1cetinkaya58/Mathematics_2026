
# Exercise 13. Determinant by Elimination

## Question

Compute the determinant

$$
A=
\begin{pmatrix}
1 & 2 & 3\\
2 & 5 & 7\\
1 & 0 & 2
\end{pmatrix}
$$

using elimination. Record the effect of every row operation used on the value of the determinant.

## Solution

### Step 1. Plan the Elimination

We will use elementary row replacement operations to transform the given matrix into an upper triangular matrix.

A row replacement operation consists of adding a multiple of one row to another row. This type of operation does not change the determinant.

We will record the effect of each row operation on the determinant.

### Step 2. Write the Given Matrix

$$
A=
\begin{pmatrix}
1 & 2 & 3\\
2 & 5 & 7\\
1 & 0 & 2
\end{pmatrix}
$$

### Step 3. Create Zeros Below the First Pivot

First, subtract twice the first row from the second row:

$$
R_2 \leftarrow R_2-2R_1
$$

The new second row is:

$$
(2,5,7)-2(1,2,3)
=(0,1,1)
$$

This row operation does not change the determinant.

Next, subtract the first row from the third row:

$$
R_3 \leftarrow R_3-R_1
$$

The new third row is:

$$
(1,0,2)-(1,2,3)
=(0,-2,-1)
$$

This row operation also does not change the determinant.

The matrix becomes:

$$
\begin{pmatrix}
1 & 2 & 3\\
0 & 1 & 1\\
0 & -2 & -1
\end{pmatrix}
$$

### Step 4. Create a Zero Below the Second Pivot

Add twice the second row to the third row:

$$
R_3 \leftarrow R_3+2R_2
$$

The new third row is:

$$
(0,-2,-1)+2(0,1,1)
=(0,0,1)
$$

This row operation also does not change the determinant.

We obtain the upper triangular matrix:

$$
\begin{pmatrix}
1 & 2 & 3\\
0 & 1 & 1\\
0 & 0 & 1
\end{pmatrix}
$$

### Step 5. Calculate the Determinant

The determinant of an upper triangular matrix is the product of its diagonal entries.

Therefore:

$$
\det(A)=1\cdot 1\cdot 1
$$

$$
\boxed{\det(A)=1}
$$

### Step 6. Final Answer and Conclusion

$$
\boxed{\det(A)=1}
$$

All three row operations used were row replacement operations. Adding a multiple of one row to another row does not change the determinant.

Therefore, the determinant remained unchanged throughout the elimination process, and the final answer is 1.
