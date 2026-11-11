
# Exercise 1. Definition of the Inverse

## Question

Given the matrices

$$
A =
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
\qquad
B =
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}
$$

Check, without using a formula, whether $B=A^{-1}$.

We calculate both $AB$ and $BA$ and compare the results with the definition of an inverse matrix.

## Step 1. Calculate $AB$

Multiply matrix $A$ by matrix $B$:

$$
AB =
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}
$$

Calculate each entry:

$$
AB =
\begin{pmatrix}
2(1)+1(-1) & 2(-1)+1(2) \\
1(1)+1(-1) & 1(-1)+1(2)
\end{pmatrix}
$$

Simplifying:

$$
AB =
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
= I
$$

## Step 2. Calculate $BA$

Now multiply matrix $B$ by matrix $A$:

$$
BA =
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
$$

Calculate each entry:

$$
BA =
\begin{pmatrix}
1(2)+(-1)(1) & 1(1)+(-1)(1) \\
(-1)(2)+2(1) & (-1)(1)+2(1)
\end{pmatrix}
$$

Simplifying:

$$
BA =
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
= I
$$

## Step 3. Conclusion

By definition, matrix $B$ is the inverse of matrix $A$ if both products equal the identity matrix:

$$
AB = BA = I
$$

We have verified that both products give the identity matrix.

Therefore:

$$
\boxed{B=A^{-1}}
$$
