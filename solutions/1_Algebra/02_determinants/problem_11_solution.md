# Exercise 11. Shortening the Calculation with Row Operations

## Question

Compute the determinant

$$
\det(A)=
\begin{vmatrix}
1 & 2 & 3\\
1 & 3 & 4\\
1 & 4 & 6
\end{vmatrix}
$$

by first performing row operations that create as many zeros as possible.

State which row operations do not change the determinant.

> **Why this exercise:** This exercise develops planning instead of mechanically repeating the same procedure.

## Solution

### Step 1. Plan the Row Operations

Before calculating the determinant, we should first create as many zeros as possible below the main diagonal. This will transform the matrix into an upper triangular matrix, whose determinant is the product of its diagonal entries.

There are three types of elementary row operations:

1. **Row replacement:** Adding a multiple of one row to another row does not change the determinant.
2. **Row interchange:** Swapping two rows changes the sign of the determinant.
3. **Row scaling:** Multiplying a row by a nonzero constant multiplies the determinant by that constant.

In this solution, we will use only row replacement operations. Therefore, the determinant will remain unchanged throughout the calculation.

### Step 2. Write the Given Matrix

$$
A=
\begin{pmatrix}
1 & 2 & 3\\
1 & 3 & 4\\
1 & 4 & 6
\end{pmatrix}
$$

### Step 3. Create Zeros in the First Column

First, subtract the first row from the second row:

$$
R_2 \rightarrow R_2-R_1
$$

Then, subtract the first row from the third row:

$$
R_3 \rightarrow R_3-R_1
$$

The matrix becomes:

$$
\begin{pmatrix}
1 & 2 & 3\\
0 & 1 & 1\\
0 & 2 & 3
\end{pmatrix}
$$

Neither operation changes the determinant because both are row replacement operations.

### Step 4. Create a Zero in the Second Column

Now subtract twice the second row from the third row:

$$
R_3 \rightarrow R_3-2R_2
$$

We obtain:

$$
\begin{pmatrix}
1 & 2 & 3\\
0 & 1 & 1\\
0 & 0 & 1
\end{pmatrix}
$$

This operation also does not change the determinant.

The matrix is now upper triangular.

### Step 5. Calculate the Determinant

The determinant of an upper triangular matrix is the product of its diagonal entries.

Therefore:

$$
\det(A)=1\cdot1\cdot1
$$

$$
\boxed{\det(A)=1}
$$

### Step 6. Final Answer and Conclusion

The final answer is:

$$
\boxed{\det(A)=1}
$$

We simplified the matrix by creating zeros below the main diagonal.

All the row operations used in this solution were row replacement operations. Adding a multiple of one row to another does not change the determinant.

Therefore, the determinant remained unchanged throughout the calculation, and the final answer is **1**.
