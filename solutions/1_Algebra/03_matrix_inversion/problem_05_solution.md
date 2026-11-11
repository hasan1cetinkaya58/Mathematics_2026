
# Exercise 5: A 3×3 Matrix

## Question

Use Gauss–Jordan elimination to find the inverse of

$$
A =
\begin{pmatrix}
1 & 1 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1
\end{pmatrix}
$$

Check the result by multiplication.

## Solution

### Step 1. Construct the Augmented Matrix

We start by writing the original matrix next to the identity matrix.

$$
[A \mid I] =
\left[
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 1 & 0 & 1 & 0 \\
1 & 0 & 1 & 0 & 0 & 1
\end{array}
\right]
$$

### Step 2. Eliminate the Entry Below the First Pivot

We apply the row operation:

$$
R_3 \rightarrow R_3 - R_1
$$

Calculation:

$$
(1,0,1,0,0,1)-(1,1,0,1,0,0)
$$

$$
R_3=(0,-1,1,-1,0,1)
$$

The new augmented matrix becomes:

$$
\left[
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 1 & 0 & 1 & 0 \\
0 & -1 & 1 & -1 & 0 & 1
\end{array}
\right]
$$

### Step 3. Eliminate the Negative One

We apply:

$$
R_3 \rightarrow R_3 + R_2
$$

Calculation:

$$
(0,-1,1,-1,0,1)+(0,1,1,0,1,0)
$$

$$
R_3=(0,0,2,-1,1,1)
$$

The new augmented matrix becomes:

$$
\left[
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 1 & 0 & 1 & 0 \\
0 & 0 & 2 & -1 & 1 & 1
\end{array}
\right]
$$

### Step 4. Make the Third Pivot Equal to 1

We divide the third row by 2.

$$
R_3 \rightarrow \frac{1}{2}R_3
$$

The new augmented matrix becomes:

$$
\left[
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 1 & 0 & 1 & 0 \\
0 & 0 & 1 & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{array}
\right]
$$

### Step 5. Eliminate the Entry Above the Third Pivot

We apply:

$$
R_2 \rightarrow R_2 - R_3
$$

Calculation:




$$
R_2 = (0,1,1,0,1,0) - \left(0,0,1,-\frac{1}{2},\frac{1}{2},\frac{1}{2}\right)
$$

$$
R_2 = \left(0,1,0,\frac{1}{2},\frac{1}{2},-\frac{1}{2}\right)
$$


The new augmented matrix becomes:

$$
\left[
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 0 & \frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
0 & 0 & 1 & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{array}
\right]
$$

### Step 6. Eliminate the Entry Above the Second Pivot

We apply:

$$
R_1 \rightarrow R_1 - R_2
$$

Calculation:

$$
R_1 = (1,1,0,1,0,0) -
\left(0,1,0,\frac{1}{2},\frac{1}{2},-\frac{1}{2}\right)
$$

$$
R_1 =
\left(1,0,0,\frac{1}{2},-\frac{1}{2},\frac{1}{2}\right)
$$

The final augmented matrix becomes:

$$
\left[
\begin{array}{ccc|ccc}
1 & 0 & 0 & \frac{1}{2} & -\frac{1}{2} & \frac{1}{2} \\
0 & 1 & 0 & \frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
0 & 0 & 1 & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{array}
\right]
$$

### Step 7. Obtain the Inverse Matrix

The left side is now the identity matrix. Therefore, the right side is the inverse of the original matrix.

$$
\boxed{
A^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} & \frac{1}{2} \\
\frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
-\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{pmatrix}
}
$$

### Step 8. Check the Result by Multiplication

We multiply the original matrix by its inverse.

$$
A \cdot A^{-1} =
\begin{pmatrix}
1 & 1 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} & \frac{1}{2} \\
\frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
-\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{pmatrix}
$$

Calculation:




$$
A \cdot A^{-1} =
\begin{pmatrix}
1 & 1 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} & \frac{1}{2} \\
\frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
-\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{pmatrix}
$$

$$
A \cdot A^{-1} =
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{pmatrix}
= I
$$

Therefore:

$$
\boxed{
A \cdot A^{-1} =
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{pmatrix}
= I
}
$$

### Final Answer

$$
\boxed{
A^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} & \frac{1}{2} \\
\frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
-\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{pmatrix}
}
$$

### Conclusion

Using Gauss–Jordan elimination, we transformed the augmented matrix from [A | I] into [I | A⁻¹].

We verified the result by multiplication. Since the product is the identity matrix, the calculated inverse is correct.
