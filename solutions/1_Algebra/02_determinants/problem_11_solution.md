# Determinants – Exercise 11

## Exercise 11. Shortening the Calculation with Row Operations

Given:

$$A=\begin{pmatrix}1&2&3\\1&3&4\\1&4&6\end{pmatrix}$$

We will create as many zeros as possible using row operations.

### Step 1: Subtract row 1 from row 2.

$$R_2\leftarrow R_2-R_1$$ $$ (1,3,4)-(1,2,3)=(0,1,1) $$

### Step 2: Subtract row 1 from row 3.

$$R_3\leftarrow R_3-R_1$$ $$ (1,4,6)-(1,2,3)=(0,2,3) $$

The resulting matrix is:

$$A'=\begin{pmatrix}1&2&3\\0&1&1\\0&2&3\end{pmatrix}$$

### Step 3: Eliminate the second entry of row 3.

$$R_3\leftarrow R_3-2R_2$$ $$ (0,2,3)-2(0,1,1)=(0,0,1) $$

The resulting matrix is:

$$A''=\begin{pmatrix}1&2&3\\0&1&1\\0&0&1\end{pmatrix}$$

### Step 4: Calculate the determinant.

The matrix is upper triangular.

$$\det(A)=1\cdot1\cdot1=\boxed{1}$$

All three row operations add a multiple of one row to another row, so
they do not change the determinant.

------------------------------------------------------------------------

