
# Exercise 7: Using Properties Instead of Recomputing

## Question

Suppose that for a $3\times3$ matrix:

$$
\det(A)=-4
$$

Compute:

$$
\det(2A),\quad \det(A^T),\quad \det(A^2),\quad \det(-A)
$$

Justify each answer using the appropriate determinant property.

## Solution

### 1. Calculate det(2A)

For an $n\times n$ matrix, multiplying the entire matrix by a scalar $k$ multiplies its determinant by $k^n$.

Since $A$ is a $3\times3$ matrix:

$$
\det(kA)=k^3\det(A)
$$

For $k=2$:

$$
\det(2A)=2^3\det(A)
$$

Substituting the given determinant:

$$
\det(2A)=8\cdot(-4)
$$

Therefore:

$$
\boxed{\det(2A)=-32}
$$

### 2. Calculate det(A^T)

The determinant of a matrix is equal to the determinant of its transpose.

The property is:

$$
\det(A^T)=\det(A)
$$

Since:

$$
\det(A)=-4
$$

Therefore:

$$
\boxed{\det(A^T)=-4}
$$

### 3. Calculate det(A^2)

The determinant of a product of two square matrices is equal to the product of their determinants.

The property is:

$$
\det(AB)=\det(A)\det(B)
$$

Since $A^2=A\cdot A$:

$$
\det(A^2)=\det(A)\cdot\det(A)
$$

Substituting the given value:

$$
\det(A^2)=(-4)\cdot(-4)
$$

Therefore:

$$
\boxed{\det(A^2)=16}
$$

### 4. Calculate det(-A)

Multiplying a $3\times3$ matrix by $-1$ multiplies its determinant by $(-1)^3$.

Using the scalar multiplication property:

$$
\det(-A)=(-1)^3\det(A)
$$

Substituting the given value:

$$
\det(-A)=(-1)\cdot(-4)
$$

Therefore:

$$
\boxed{\det(-A)=4}
$$

### 5. Final Conclusion

Using the properties of determinants, we obtain:

$$
\boxed{\det(2A)=-32}
$$

$$
\boxed{\det(A^T)=-4}
$$

$$
\boxed{\det(A^2)=16}
$$

$$
\boxed{\det(-A)=4}
$$

These results demonstrate that determinant properties allow us to calculate the determinants of transformed matrices without performing a complete determinant expansion.
