# Determinants – Exercise 15

## Exercise 15. Combining Determinant Properties

Given:

$$\det(A)=-2,\qquad\det(B)=3$$

Matrices A and B are invertible 2×2 matrices. We need to calculate:

$$\det(B^{-1}A^TB)$$

### Step 1: Apply the product property.

$$\det(B^{-1}A^TB)=\det(B^{-1})\det(A^T)\det(B)$$

### Step 2: Apply the inverse determinant property.

$$\det(B^{-1})=\frac{1}{\det(B)}=\frac13$$

### Step 3: Apply the transpose determinant property.

$$\det(A^T)=\det(A)=-2$$

### Step 4: Substitute the values.

$$\det(B^{-1}A^TB)=\frac13\cdot(-2)\cdot3$$ $$=1\cdot(-2)$$
$$\boxed{\det(B^{-1}A^TB)=-2}$$

### Step 5: Explain why the B factors cancel.

$$\det(B^{-1})\det(B)=\frac{1}{\det(B)}\cdot\det(B)=1$$

The factors involving B cancel each other, leaving only the determinant
of A.

**Final Answer:** $\boxed{-2}$


