
# Exercise 2. Formula for a 2×2 Matrix

## Question

Find the inverse of

$$
A =
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix}
$$

using the formula for a $2\times2$ matrix. At the end, check the result by computing one product with $A$.

## Step 1. Write the Inverse Matrix Formula

For a $2\times2$ matrix

$$
A =
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
$$

the inverse is given by

$$
A^{-1} =
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
$$

provided that $ad-bc\neq 0$.

## Step 2. Calculate the Determinant

For the given matrix,

$$
a=3,\quad b=2,\quad c=5,\quad d=4
$$

The determinant is

$$
\det(A)=ad-bc
$$

Substituting the values:

$$
\det(A)=3\cdot4-2\cdot5
$$

$$
\det(A)=12-10=2
$$

Since the determinant is not zero, the inverse matrix exists.

## Step 3. Apply the Formula

Using the inverse matrix formula:

$$
A^{-1}=
\frac{1}{2}
\begin{pmatrix}
4 & -2 \\
-5 & 3
\end{pmatrix}
$$

Multiply each entry by $\frac{1}{2}$:

$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}
$$

## Step 4. Verify the Result

To check the result, calculate $AA^{-1}$:

$$
AA^{-1}=
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}
$$

Calculate each entry:

$$
AA^{-1}=
\begin{pmatrix}
3(2)+2\left(-\frac{5}{2}\right) &
3(-1)+2\left(\frac{3}{2}\right) \\[6pt]
5(2)+4\left(-\frac{5}{2}\right) &
5(-1)+4\left(\frac{3}{2}\right)
\end{pmatrix}
$$

Simplifying:

$$
AA^{-1}=
\begin{pmatrix}
6-5 & -3+3 \\
10-10 & -5+6
\end{pmatrix}
$$

Therefore,

$$
AA^{-1}=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
=I
$$

## Step 5. Conclusion

The determinant of $A$ is non-zero, so the inverse exists.

The verification gives the identity matrix:

$$
AA^{-1}=I
$$

Therefore, the inverse matrix is

$$
\boxed{
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}
}
$$
