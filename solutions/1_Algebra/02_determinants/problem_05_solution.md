
# Exercise 5: Row Operations

## Question

Given the matrix:

$$
A=
\begin{pmatrix}
1 & 2 & 3\\
2 & 1 & 0\\
-1 & 4 & 2
\end{pmatrix}
$$

Find the determinant by simplifying the matrix with row operations. At each step, indicate whether and how the determinant changes.

## Solution

### 1. Write the Original Matrix

We are given:

$$
A=
\begin{pmatrix}
1 & 2 & 3\\
2 & 1 & 0\\
-1 & 4 & 2
\end{pmatrix}
$$

Our goal is to simplify the matrix into an upper triangular form using elementary row operations.

We will use row replacement operations, which do not change the determinant.

### 2. Eliminate the First Entry in the Second Row

Apply the row operation:

$$
R_2 \rightarrow R_2-2R_1
$$

The new second row is:

$$
(2,1,0)-2(1,2,3)
$$

$$
=(2,1,0)-(2,4,6)
$$

$$
=(0,-3,-6)
$$

The resulting matrix is:

$$
A_1=
\begin{pmatrix}
1 & 2 & 3\\
0 & -3 & -6\\
-1 & 4 & 2
\end{pmatrix}
$$

**Effect on the determinant:**

Adding a multiple of one row to another row does not change the determinant.

Therefore:

$$
\det(A_1)=\det(A)
$$

### 3. Eliminate the First Entry in the Third Row

Apply the row operation:

$$
R_3 \rightarrow R_3+R_1
$$

The new third row is:

$$
(-1,4,2)+(1,2,3)
$$

$$
=(0,6,5)
$$

The resulting matrix is:

$$
A_2=
\begin{pmatrix}
1 & 2 & 3\\
0 & -3 & -6\\
0 & 6 & 5
\end{pmatrix}
$$

**Effect on the determinant:**

This is also a row replacement operation, so the determinant does not change.

Therefore:

$$
\det(A_2)=\det(A_1)=\det(A)
$$

### 4. Eliminate the Second Entry in the Third Row

Apply the row operation:

$$
R_3 \rightarrow R_3+2R_2
$$

The new third row is:

$$
(0,6,5)+2(0,-3,-6)
$$

$$
=(0,6,5)+(0,-6,-12)
$$

$$
=(0,0,-7)
$$

The resulting matrix is:

$$
A_3=
\begin{pmatrix}
1 & 2 & 3\\
0 & -3 & -6\\
0 & 0 & -7
\end{pmatrix}
$$

**Effect on the determinant:**

Adding a multiple of one row to another does not change the determinant.

Therefore:

$$
\det(A_3)=\det(A_2)=\det(A)
$$

### 5. Calculate the Determinant

The resulting matrix is upper triangular.

The determinant of an upper triangular matrix is the product of its main diagonal entries.

Therefore:

$$
\det(A_3)=1\cdot(-3)\cdot(-7)
$$

$$
\det(A_3)=21
$$

Since none of our row operations changed the determinant:

$$
\det(A)=\det(A_3)
$$

Thus:

$$
\boxed{\det(A)=21}
$$

## 6. Final Conclusion

We simplified the original matrix into an upper triangular matrix using three row replacement operations.

At every step, we added a multiple of one row to another row. These operations do not change the determinant.

The final determinant is:

$$
\boxed{\det(A)=21}
$$

This exercise demonstrates how elementary row operations can simplify determinant calculations while preserving the determinant, provided that the effect of each operation is correctly tracked.
