# Determinants – Exercise 5

## Exercise 5. Row Operations

Given:

$$A=\begin{pmatrix}1&2&3\\2&1&0\\-1&4&2\end{pmatrix}$$

We will use row operations to create zeros.

### Step 1: Eliminate the first entry of row 2.

$$R_2\leftarrow R_2-2R_1$$ $$ (2,1,0)-2(1,2,3)=(0,-3,-6) $$

Adding a multiple of one row to another row does not change the
determinant.

### Step 2: Eliminate the first entry of row 3.

$$R_3\leftarrow R_3+R_1$$ $$(-1,4,2)+(1,2,3)=(0,6,5)$$

The determinant does not change. The resulting matrix is:

$$A'=\begin{pmatrix}1&2&3\\0&-3&-6\\0&6&5\end{pmatrix}$$

### Step 3: Expand along the first column.

$$\det(A)=1\begin{vmatrix}-3&-6\\6&5\end{vmatrix}$$
$$=(-3)\cdot5-(-6)\cdot6=-15+36$$ $$\boxed{\det(A)=21}$$

**Row operation rule:** $R_i\leftarrow R_i+kR_j$ does not change the
determinant.

------------------------------------------------------------------------

