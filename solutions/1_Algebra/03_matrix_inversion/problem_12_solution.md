# Exercise 12. Finding Inverses Without Starting from Scratch

## Question

**Given:**

It is known that

$$A^{-1} = \begin{bmatrix} 2 & -1 \\ -3 & 2 \end{bmatrix}$$

**Required:**

Without finding $A$:

1. Compute $(3A)^{-1}$.
2. Compute $(A^T)^{-1}$.
3. Compute $(A^2)^{-1}$.
4. Justify each result using the appropriate property.

> **Why this exercise:** Teaches how to use inverse properties instead of carrying out unnecessary full calculations.

---

## Solution

### Step 1. Calculate the Inverse of $3A$

We use the scalar multiplication property of inverse matrices, which states that for any non-zero scalar $c$:

$$(cA)^{-1} = \frac{1}{c}A^{-1}$$

Since the scalar is $c = 3$, we obtain:

$$(3A)^{-1} = \frac{1}{3}A^{-1}$$

Substituting the given inverse matrix $A^{-1}$:

$$(3A)^{-1} = \frac{1}{3} \begin{bmatrix} 2 & -1 \\ -3 & 2 \end{bmatrix}$$

Therefore:

$$(3A)^{-1} = \begin{bmatrix} \frac{2}{3} & -\frac{1}{3} \\ -1 & \frac{2}{3} \end{bmatrix}$$

### Step 2. Calculate the Inverse of $A$ Transpose

We use the transpose property of inverse matrices:

$$(A^T)^{-1} = (A^{-1})^T$$

This means we transpose the given inverse matrix by switching its rows and columns:

$$(A^T)^{-1} = \begin{bmatrix} 2 & -1 \\ -3 & 2 \end{bmatrix}^T = \begin{bmatrix} 2 & -3 \\ -1 & 2 \end{bmatrix}$$

### Step 3. Calculate the Inverse of $A$ Squared

We use the power property of inverse matrices, which states that for any positive integer $k$:

$$(A^k)^{-1} = (A^{-1})^k$$

For $k = 2$, we obtain:

$$(A^2)^{-1} = (A^{-1})^2$$

Therefore:

$$(A^2)^{-1} = \begin{bmatrix} 2 & -1 \\ -3 & 2 \end{bmatrix} \begin{bmatrix} 2 & -1 \\ -3 & 2 \end{bmatrix}$$

Multiplying the matrices:

$$(A^2)^{-1} = \begin{bmatrix} 2 \cdot 2 + (-1) \cdot (-3) & 2 \cdot (-1) + (-1) \cdot 2 \\ (-3) \cdot 2 + 2 \cdot (-3) & (-3) \cdot (-1) + 2 \cdot 2 \end{bmatrix}$$

Simplifying:

$$(A^2)^{-1} = \begin{bmatrix} 7 & -4 \\ -12 & 7 \end{bmatrix}$$

### Final Answer

The three results are:

**1. Inverse of $3A$**

$$(3A)^{-1} = \begin{bmatrix} \frac{2}{3} & -\frac{1}{3} \\ -1 & \frac{2}{3} \end{bmatrix}$$

**2. Inverse of $A$ Transpose**

$$(A^T)^{-1} = \begin{bmatrix} 2 & -3 \\ -1 & 2 \end{bmatrix}$$

**3. Inverse of $A$ Squared**

$$(A^2)^{-1} = \begin{bmatrix} 7 & -4 \\ -12 & 7 \end{bmatrix}$$

### Conclusion

We used three important properties of inverse matrices:

1. The inverse of a scalar multiple is the inverse matrix multiplied by the reciprocal of the scalar: $(cA)^{-1} = \frac{1}{c}A^{-1}$.
2. The inverse of a transpose is the transpose of the inverse: $(A^T)^{-1} = (A^{-1})^T$.
3. The inverse of a matrix power is the corresponding power of the inverse matrix: $(A^k)^{-1} = (A^{-1})^k$.

These properties allow us to calculate all three results without finding the original matrix $A$.
