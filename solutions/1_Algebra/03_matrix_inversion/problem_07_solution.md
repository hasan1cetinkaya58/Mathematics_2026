
# Exercise 7: Inverse of a Product

## Question

For the matrices

$$
A =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix},
\qquad
B =
\begin{pmatrix}
2 & 0 \\
0 & 3
\end{pmatrix}
$$

Compute:

1. $(AB)^{-1}$

2. $B^{-1}A^{-1}$

Check that the results are the same and explain the meaning of the reversed order.

## Solution

### Step 1. Calculate the Product AB

First, we multiply matrix A by matrix B.

$$
AB =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 3
\end{pmatrix}
$$

Calculation:

$$
AB =
\begin{pmatrix}
1\cdot2+1\cdot0 & 1\cdot0+1\cdot3 \\
0\cdot2+1\cdot0 & 0\cdot0+1\cdot3
\end{pmatrix}
$$

$$
AB =
\begin{pmatrix}
2 & 3 \\
0 & 3
\end{pmatrix}
$$

### Step 2. Calculate the Determinant of AB

Before finding the inverse, we calculate the determinant.

$$
\det(AB) =
\begin{vmatrix}
2 & 3 \\
0 & 3
\end{vmatrix}
$$

Calculation:

$$
\det(AB) = 2\cdot3-3\cdot0
$$

$$
\det(AB)=6
$$

Since the determinant is not zero, the inverse exists.

### Step 3. Find the Inverse of AB

We use the inverse formula for a 2×2 matrix:

$$
M^{-1} =
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
$$

Applying this formula:

$$
(AB)^{-1} =
\frac{1}{6}
\begin{pmatrix}
3 & -3 \\
0 & 2
\end{pmatrix}
$$

Therefore:

$$
\boxed{
(AB)^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
}
$$

### Step 4. Find the Inverse of A and B Separately

First, we calculate the inverse of matrix A.

$$
A^{-1} =
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

Next, we calculate the inverse of matrix B.

$$
B^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & \frac{1}{3}
\end{pmatrix}
$$

### Step 5. Calculate B⁻¹A⁻¹

We multiply the inverse of B by the inverse of A.

$$
B^{-1}A^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & \frac{1}{3}
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

Calculation:

$$
B^{-1}A^{-1} =
\begin{pmatrix}
\frac{1}{2}\cdot1+0\cdot0 &
\frac{1}{2}\cdot(-1)+0\cdot1 \\
0\cdot1+\frac{1}{3}\cdot0 &
0\cdot(-1)+\frac{1}{3}\cdot1
\end{pmatrix}
$$

$$
B^{-1}A^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
$$

### Step 6. Compare the Results

We compare the two inverse matrices.

$$
(AB)^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
$$

$$
B^{-1}A^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
$$

Therefore:

$$
\boxed{(AB)^{-1}=B^{-1}A^{-1}}
$$

The results are exactly the same.

### Step 7. Explain the Reversed Order

The inverse of a product reverses the order of the matrices.

In general:

$$
\boxed{(AB)^{-1}=B^{-1}A^{-1}}
$$

This means that when we reverse a product, we must also reverse the order of the inverse matrices.

The reason is that the inverse operation must undo the original multiplication in reverse order.

### Final Answer

$$
\boxed{
(AB)^{-1}=B^{-1}A^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
}
$$

### Conclusion

We calculated the inverse of the product AB and separately calculated B⁻¹A⁻¹.

Both calculations gave the same result.

This confirms the important matrix property that the inverse of a product is equal to the product of the inverses in reversed order.
