# Determinants – Exercise 13

## Exercise 13. Determinant by Elimination

Given:

$$A=\begin{pmatrix}1&2&3\\2&5&7\\1&0&2\end{pmatrix}$$

We will calculate the determinant using elimination.

### Step 1: Eliminate the first entry of row 2.

$$R_2\leftarrow R_2-2R_1$$ $$ (2,5,7)-2(1,2,3)=(0,1,1) $$

### Step 2: Eliminate the first entry of row 3.

$$R_3\leftarrow R_3-R_1$$ $$ (1,0,2)-(1,2,3)=(0,-2,-1) $$

The new matrix is:

$$A'=\begin{pmatrix}1&2&3\\0&1&1\\0&-2&-1\end{pmatrix}$$

### Step 3: Eliminate the second entry of row 3.

$$R_3\leftarrow R_3+2R_2$$ $$ (0,-2,-1)+2(0,1,1)=(0,0,1) $$

The new matrix is:

$$A''=\begin{pmatrix}1&2&3\\0&1&1\\0&0&1\end{pmatrix}$$

### Step 4: Calculate the determinant.

The matrix is upper triangular.

$$\det(A)=1\cdot1\cdot1=\boxed{1}$$

**Effect of each row operation:**

-   $R_2\leftarrow R_2-2R_1$: The determinant does not change.
-   $R_3\leftarrow R_3-R_1$: The determinant does not change.
-   $R_3\leftarrow R_3+2R_2$: The determinant does not change.

Therefore, the determinant of the original matrix is also 1.

------------------------------------------------------------------------

