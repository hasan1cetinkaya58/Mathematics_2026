
# Exercise 8: Determinant of a Product

## Question

Let A and B be square matrices such that:

$$
\det(A)=3,\qquad \det(B)=-5
$$

Compute:

$$
\det(AB),\quad \det(BA),\quad \det(A^{-1}B)
$$

Explain why the first two results are equal even though usually AB is not equal to BA.

## Solution

### 1. Calculate det(AB)

The determinant of a product of two square matrices is equal to the product of their determinants.

The property is:

$$
\det(AB)=\det(A)\cdot\det(B)
$$

Substituting the given values:

$$
\det(AB)=3\cdot(-5)
$$

Therefore:

$$
\boxed{\det(AB)=-15}
$$

### 2. Calculate det(BA)

Using the same determinant property:

$$
\det(BA)=\det(B)\cdot\det(A)
$$

Substituting:

$$
\det(BA)=(-5)\cdot3
$$

Therefore:

$$
\boxed{\det(BA)=-15}
$$

### 3. Calculate det(A^{-1}B)

First, we check whether the inverse of A exists.

A square matrix is invertible if and only if its determinant is nonzero.

Since:

$$
\det(A)=3\neq0
$$

The inverse matrix A^{-1} exists.

The determinant of an inverse matrix satisfies:

$$
\det(A^{-1})=\frac{1}{\det(A)}
$$

Therefore:

$$
\det(A^{-1})=\frac{1}{3}
$$

Using the product property:

$$
\det(A^{-1}B)=\det(A^{-1})\cdot\det(B)
$$

Substituting the values:

$$
\det(A^{-1}B)=\frac{1}{3}\cdot(-5)
$$

Therefore:

$$
\boxed{\det(A^{-1}B)=-\frac{5}{3}}
$$

### 4. Explain Why det(AB) = det(BA)

In general, matrix multiplication is not commutative.

This means:

$$
AB\neq BA
$$

However, the determinant of a product satisfies:

$$
\det(AB)=\det(A)\cdot\det(B)
$$

and

$$
\det(BA)=\det(B)\cdot\det(A)
$$

Since multiplication of real numbers is commutative:

$$
\det(A)\cdot\det(B)=\det(B)\cdot\det(A)
$$

Therefore:

$$
\boxed{\det(AB)=\det(BA)}
$$

Both determinants are equal even though the matrices AB and BA are generally different.

### 5. Final Conclusion

Using the properties of determinants, we obtain:

$$
\boxed{\det(AB)=-15}
$$

$$
\boxed{\det(BA)=-15}
$$

$$
\boxed{\det(A^{-1}B)=-\frac{5}{3}}
$$

The inverse of A exists because its determinant is nonzero.

This exercise demonstrates that determinants behave consistently under matrix multiplication and inversion, even when matrix multiplication itself is not commutative.
