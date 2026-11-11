
# Exercise 6: Solving a System Using the Inverse

## Question

Solve

$$
Ax=b
$$

where

$$
A=
\begin{pmatrix}
2 & 1\\
1 & 3
\end{pmatrix},
\qquad
b=
\begin{pmatrix}
5\\
7
\end{pmatrix}
$$

using

$$
x=A^{-1}b
$$

Then substitute the resulting vector back into the equation and check the result.

## Solution

### Step 1. Calculate the Determinant of A

First, we calculate the determinant to make sure that the inverse exists.

$$
\det(A)=
\begin{vmatrix}
2 & 1\\
1 & 3
\end{vmatrix}
$$

Calculation:

$$
\det(A)=(2\cdot3)-(1\cdot1)
$$

$$
\det(A)=6-1=5
$$

Since the determinant is not zero, the inverse of A exists.

### Step 2. Find the Inverse Matrix

For a 2×2 matrix, the inverse formula is:

$$
A^{-1}=
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b\\
-c & a
\end{pmatrix}
$$

Using the values from matrix A:

$$
A^{-1}=
\frac{1}{5}
\begin{pmatrix}
3 & -1\\
-1 & 2
\end{pmatrix}
$$

Therefore:

$$
A^{-1}=
\begin{pmatrix}
\frac{3}{5} & -\frac{1}{5}\\
-\frac{1}{5} & \frac{2}{5}
\end{pmatrix}
$$

### Step 3. Calculate x Using x = A⁻¹b

We use the formula:

$$
x=A^{-1}b
$$

Substituting the inverse matrix and vector b:

$$
x=
\begin{pmatrix}
\frac{3}{5} & -\frac{1}{5}\\
-\frac{1}{5} & \frac{2}{5}
\end{pmatrix}
\begin{pmatrix}
5\\
7
\end{pmatrix}
$$

Calculation:

$$
x=
\begin{pmatrix}
\frac{3}{5}\cdot5-\frac{1}{5}\cdot7\\
-\frac{1}{5}\cdot5+\frac{2}{5}\cdot7
\end{pmatrix}
$$

$$
x=
\begin{pmatrix}
\frac{15}{5}-\frac{7}{5}\\
-\frac{5}{5}+\frac{14}{5}
\end{pmatrix}
$$

$$
x=
\begin{pmatrix}
\frac{8}{5}\\
\frac{9}{5}
\end{pmatrix}
$$

### Step 4. Substitute the Result into the Original Equation

To check the solution, we substitute the calculated vector x into Ax = b.

$$
Ax=
\begin{pmatrix}
2 & 1\\
1 & 3
\end{pmatrix}
\begin{pmatrix}
\frac{8}{5}\\
\frac{9}{5}
\end{pmatrix}
$$

Calculation:

$$
Ax =
\begin{pmatrix}
2\cdot\frac{8}{5}+1\cdot\frac{9}{5}\\
1\cdot\frac{8}{5}+3\cdot\frac{9}{5}
\end{pmatrix}
$$

$$
Ax =
\begin{pmatrix}
\frac{16}{5}+\frac{9}{5}\\
\frac{8}{5}+\frac{27}{5}
\end{pmatrix}
$$

$$
Ax =
\begin{pmatrix}
\frac{25}{5}\\
\frac{35}{5}
\end{pmatrix}
$$

$$
Ax =
\begin{pmatrix}
5\\
7
\end{pmatrix}
$$

Since the result is equal to the original vector b, the solution is correct.

### Final Answer

$$
\boxed{
x=
\begin{pmatrix}
\frac{8}{5}\\
\frac{9}{5}
\end{pmatrix}
}
$$

### Conclusion

The inverse matrix method was used to solve the linear system.

First, we calculated the inverse of A because its determinant was not zero.

Then, we used the formula x = A⁻¹b to find the solution.

Finally, we substituted the calculated vector into the original equation Ax = b.

Since the result equals b, the solution is verified and correct.
