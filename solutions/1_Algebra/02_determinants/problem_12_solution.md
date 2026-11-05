# Determinants – Exercise 12

## Exercise 12. A Parameter Revealed by a Row Operation

Given:

$$A(t)=\begin{pmatrix}1&2&3\\2&4&t\\0&1&1\end{pmatrix}$$

### Step 1: Apply the given row operation.

$$R_2\leftarrow R_2-2R_1$$

$$ (2,4,t)-2(1,2,3)=(2,4,t)-(2,4,6)=(0,0,t-6) $$

The new matrix is:

$$A'=\begin{pmatrix}1&2&3\\0&0&t-6\\0&1&1\end{pmatrix}$$

This row operation does not change the determinant.

### Step 2: Expand along the first column.

$$\det(A)=1\begin{vmatrix}0&t-6\\1&1\end{vmatrix}$$

$$=1[0\cdot1-(t-6)\cdot1]=-(t-6)=6-t$$

Therefore, $\det(A)=6-t$.

### Step 3: Set the determinant equal to zero.

$$6-t=0$$ $$\boxed{t=6}$$

### Step 4: Explain what happens to the rows.

When $t=6$, the second row of the transformed matrix becomes:

$$R_2=(0,0,6-6)=(0,0,0)$$

In the original matrix, $R_2=(2,4,6)=2R_1$. Therefore, the first and
second rows are linearly dependent.

**Final Answer:** $\boxed{t=6}$. For this value, the determinant is zero
and the matrix is not invertible.

------------------------------------------------------------------------

