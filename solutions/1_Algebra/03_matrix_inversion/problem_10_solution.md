
# Exercise 10. Inverse of a Diagonal Matrix

## Question

Given

$$
D =
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5
\end{pmatrix},
\qquad
E =
\begin{pmatrix}
2 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 5
\end{pmatrix}
$$

Without using Gauss-Jordan elimination, decide which matrix is invertible. For the invertible matrix, give the inverse and check the result by multiplication.

## Solution

### Step 1. Determine Which Matrix Is Invertible

A diagonal matrix is invertible if all its diagonal entries are nonzero.

For matrix $D$, the diagonal entries are $2$, $-3$, and $5$. All of them are nonzero.

Therefore, $D$ is invertible.

For matrix $E$, the diagonal entries are $2$, $0$, and $5$. Since one diagonal entry is zero, $E$ is not invertible.

### Step 2. Find the Inverse of D

To find the inverse of a diagonal matrix, we take the reciprocal of each diagonal entry.

Therefore:

$$
D^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5}
\end{pmatrix}
$$

### Step 3. Check the Result by Multiplication

We multiply $D$ by $D^{-1}$:

$$
DD^{-1} =
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5}
\end{pmatrix}
$$

Multiplying the corresponding diagonal entries:

$$
DD^{-1} =
\begin{pmatrix}
2\cdot\frac{1}{2} & 0 & 0 \\
0 & (-3)\cdot(-\frac{1}{3}) & 0 \\
0 & 0 & 5\cdot\frac{1}{5}
\end{pmatrix}
$$

$$
DD^{-1} =
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{pmatrix}
= I
$$

The result is the identity matrix, so the inverse is correct.

### Final Answer

$$
\boxed{
D^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5}
\end{pmatrix}
}
$$

Matrix $D$ is invertible, while matrix $E$ is not invertible.

### Conclusion

A diagonal matrix is invertible if and only if all its diagonal entries are nonzero. Its inverse is obtained by taking the reciprocal of each diagonal entry.

The multiplication check confirms that $DD^{-1}=I$.
