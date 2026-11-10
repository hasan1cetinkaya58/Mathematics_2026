# Exercise 8: Row Operations and Their Reversibility

## Question

For the matrix

$$
A=
\begin{pmatrix}
1&2&-1\\
2&4&1\\
-1&1&3
\end{pmatrix}
$$

perform the following row operations in order:

1. $R_2 \leftarrow R_2-2R_1$
2. $R_3 \leftarrow R_3+R_1$
3. Interchange $R_2$ and $R_3$.

Write the matrix after each step. Then state an operation that reverses each of the three operations.

## Solution

### 1. Understanding Elementary Row Operations

Elementary row operations are transformations that change the rows of a matrix.

There are three types of elementary row operations:

- Interchanging two rows.
- Multiplying a row by a nonzero scalar.
- Adding a multiple of one row to another row.

Each elementary row operation is reversible. This means that an inverse operation can restore the matrix to its previous state.

The given matrix is:

$$
A=
\begin{pmatrix}
1&2&-1\\
2&4&1\\
-1&1&3
\end{pmatrix}
$$

### 2. First Row Operation

The first operation is:

$$
R_2 \leftarrow R_2-2R_1
$$

This means that we subtract twice the first row from the second row.

The original rows are:

$$
R_1=(1,2,-1)
$$

$$
R_2=(2,4,1)
$$

We calculate the new second row:

$$
\begin{aligned}
R_2&=(2,4,1)-2(1,2,-1)\\
&=(2,4,1)-(2,4,-2)\\
&=(0,0,3)
\end{aligned}
$$

The first and third rows remain unchanged.

Therefore, the matrix after the first operation is:

$$
A_1=
\begin{pmatrix}
1&2&-1\\
0&0&3\\
-1&1&3
\end{pmatrix}
$$

**Inverse operation:**

To reverse this operation, we add twice the first row to the second row:

$$
\boxed{R_2 \leftarrow R_2+2R_1}
$$

### 3. Second Row Operation

The second operation is:

$$
R_3 \leftarrow R_3+R_1
$$

We add the first row to the third row.

Using the matrix obtained after the first operation:

$$
R_3=(-1,1,3)+(1,2,-1)
$$

Calculating each entry:

$$
\begin{aligned}
R_3&=(-1+1,\ 1+2,\ 3-1)\\
&=(0,3,2)
\end{aligned}
$$

The first and second rows remain unchanged.

Therefore, the matrix after the second operation is:

$$
A_2=
\begin{pmatrix}
1&2&-1\\
0&0&3\\
0&3&2
\end{pmatrix}
$$

**Inverse operation:**

To reverse this operation, we subtract the first row from the third row:

$$
\boxed{R_3 \leftarrow R_3-R_1}
$$

### 4. Third Row Operation: Interchanging Rows

The third operation is to interchange the second and third rows:

$$
R_2 \leftrightarrow R_3
$$

Before the interchange, the matrix is:

$$
A_2=
\begin{pmatrix}
1&2&-1\\
0&0&3\\
0&3&2
\end{pmatrix}
$$

We exchange the second and third rows.

The first row remains unchanged, while the second and third rows switch positions.

Therefore, the final matrix is:

$$
A_3=
\begin{pmatrix}
1&2&-1\\
0&3&2\\
0&0&3
\end{pmatrix}
$$

**Inverse operation:**

Interchanging the same two rows again returns the matrix to its previous state.

Therefore, the inverse operation is:

$$
\boxed{R_2 \leftrightarrow R_3}
$$

### 5. Summary of All Row Operations

The complete sequence of operations is:

**Initial matrix:**

$$
A=
\begin{pmatrix}
1&2&-1\\
2&4&1\\
-1&1&3
\end{pmatrix}
$$

**After the first operation:**

$$
R_2 \leftarrow R_2-2R_1
$$

$$
A_1=
\begin{pmatrix}
1&2&-1\\
0&0&3\\
-1&1&3
\end{pmatrix}
$$

**After the second operation:**

$$
R_3 \leftarrow R_3+R_1
$$

$$
A_2=
\begin{pmatrix}
1&2&-1\\
0&0&3\\
0&3&2
\end{pmatrix}
$$

**After the third operation:**

$$
R_2 \leftrightarrow R_3
$$

$$
A_3=
\begin{pmatrix}
1&2&-1\\
0&3&2\\
0&0&3
\end{pmatrix}
$$

### 6. Inverse Operations

Each operation has an inverse that restores the matrix to its previous state.

| Original operation | Inverse operation |
|---|---|
| $R_2 \leftarrow R_2-2R_1$ | $R_2 \leftarrow R_2+2R_1$ |
| $R_3 \leftarrow R_3+R_1$ | $R_3 \leftarrow R_3-R_1$ |
| $R_2 \leftrightarrow R_3$ | $R_2 \leftrightarrow R_3$ |

To restore the original matrix from the final matrix, the inverse operations must be performed in reverse order.

**Step 1:**

Interchange the second and third rows:

$$
R_2 \leftrightarrow R_3
$$

**Step 2:**

Subtract the first row from the third row:

$$
R_3 \leftarrow R_3-R_1
$$

**Step 3:**

Add twice the first row to the second row:

$$
R_2 \leftarrow R_2+2R_1
$$

After these three inverse operations, we obtain the original matrix:

$$
\begin{pmatrix}
1&2&-1\\
2&4&1\\
-1&1&3
\end{pmatrix}
$$

This confirms that all three row operations are reversible.

### 7. Final Answer and Conclusion

The final matrix after performing all three row operations is:

$$
\boxed{
A_3=
\begin{pmatrix}
1&2&-1\\
0&3&2\\
0&0&3
\end{pmatrix}
}
$$

The inverse operations are:

$$
\boxed{
\begin{aligned}
R_2&\leftarrow R_2+2R_1\\
R_3&\leftarrow R_3-R_1\\
R_2&\leftrightarrow R_3
\end{aligned}
}
$$

**Conclusion:**

Elementary row operations are reversible transformations of a matrix. Each operation has a corresponding inverse operation that restores the previous matrix.

The order of operations is important because the inverse operations must be applied in reverse order to recover the original matrix.

This exercise demonstrates how elementary row operations can transform a matrix while preserving the ability to return to its original form.
