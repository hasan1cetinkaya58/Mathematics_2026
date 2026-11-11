# Exercise 15. Combining Determinant Properties

## Question

Let `A` and `B` be invertible `2×2` matrices with

$$
\det(A)=-2,\qquad \det(B)=3.
$$

Without finding the entries of the matrices, compute

$$
\det(B^{-1}A^TB).
$$

Apply determinant properties in order and explain why the factors involving `B` eventually cancel.

## Solution

### Step 1. Apply the Product Property

The determinant of a product of square matrices equals the product of their determinants.

Therefore,

$$
\det(B^{-1}A^TB)
=
\det(B^{-1})\det(A^T)\det(B).
$$

This is the product property of determinants.

### Step 2. Apply the Inverse Matrix Property

For an invertible matrix `B`, the determinant of its inverse is the reciprocal of its determinant:

$$
\det(B^{-1})=\frac{1}{\det(B)}.
$$

Since

$$
\det(B)=3,
$$

we obtain

$$
\det(B^{-1})=\frac{1}{3}.
$$

### Step 3. Apply the Transpose Property

The determinant of a matrix is equal to the determinant of its transpose:

$$
\det(A^T)=\det(A).
$$

Since

$$
\det(A)=-2,
$$

we obtain

$$
\det(A^T)=-2.
$$

### Step 4. Substitute and Simplify

Using the values obtained in Steps 2 and 3, we substitute into the expression from Step 1:

$$
\begin{aligned}
\det(B^{-1}A^TB)
&=\det(B^{-1})\det(A^T)\det(B)\\
&=\frac{1}{3}\cdot(-2)\cdot 3\\
&=1\cdot(-2)\\
&=-2.
\end{aligned}
$$

The factors involving `B` cancel because

$$
\det(B^{-1})\det(B)
=
\frac{1}{3}\cdot 3
=
1.
$$

### Step 5. Final Answer and Conclusion

Therefore, the final answer is

$$
\boxed{\det(B^{-1}A^TB)=-2}.
$$

The determinant properties were applied in the following order:

1. **Product property:** The determinant of a product equals the product of the determinants.
2. **Inverse property:** The determinant of an inverse matrix is the reciprocal of the original determinant.
3. **Transpose property:** The determinant of a transpose equals the determinant of the original matrix.

The factors involving `B` cancel because the determinant of `B^{-1}` is the reciprocal of the determinant of `B`. Their product is equal to `1`.

Therefore, the final determinant depends only on `det(A)`, and its value is `-2`.
