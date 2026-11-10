
# Exercise 14: Rotation Matrices

## Question

The matrix for a rotation through an angle θ is:

$$
R(\theta)=
\begin{pmatrix}
\cos\theta&-\sin\theta\\
\sin\theta&\cos\theta
\end{pmatrix}
$$

Compute R(α)R(β) and, using the angle-sum formulas for sine and cosine, show that:

$$
R(\alpha)R(\beta)=R(\alpha+\beta)
$$

Explain the result geometrically.

## Solution

### 1. Identify the Rotation Matrices

We are given two rotation matrices:

$$
R(\alpha)=
\begin{pmatrix}
\cos\alpha&-\sin\alpha\\
\sin\alpha&\cos\alpha
\end{pmatrix}
$$

$$
R(\beta)=
\begin{pmatrix}
\cos\beta&-\sin\beta\\
\sin\beta&\cos\beta
\end{pmatrix}
$$

Our goal is to multiply these matrices and prove that their product is the rotation matrix for the sum of the two angles.

### 2. Calculate the Matrix Product

By matrix multiplication:

$$
R(\alpha)R(\beta)
$$

Substituting the matrices:

$$
=
\begin{pmatrix}
\cos\alpha&-\sin\alpha\\
\sin\alpha&\cos\alpha
\end{pmatrix}
\begin{pmatrix}
\cos\beta&-\sin\beta\\
\sin\beta&\cos\beta
\end{pmatrix}
$$

### 3. Calculate Each Entry

First row, first column:

$$
\cos\alpha\cos\beta-\sin\alpha\sin\beta
$$

First row, second column:

$$
-\cos\alpha\sin\beta-\sin\alpha\cos\beta
$$

Second row, first column:

$$
\sin\alpha\cos\beta+\cos\alpha\sin\beta
$$

Second row, second column:

$$
-\sin\alpha\sin\beta+\cos\alpha\cos\beta
$$

Therefore, the product becomes:

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha\cos\beta-\sin\alpha\sin\beta&
-\cos\alpha\sin\beta-\sin\alpha\cos\beta\\
\sin\alpha\cos\beta+\cos\alpha\sin\beta&
\cos\alpha\cos\beta-\sin\alpha\sin\beta
\end{pmatrix}
$$

### 4. Apply the Angle-Sum Formulas

We use the following trigonometric identities:

Cosine angle-sum formula:

$$
\cos(\alpha+\beta)=
\cos\alpha\cos\beta-\sin\alpha\sin\beta
$$

Sine angle-sum formula:

$$
\sin(\alpha+\beta)=
\sin\alpha\cos\beta+\cos\alpha\sin\beta
$$

These identities allow us to simplify the matrix entries.

### 5. Substitute the Trigonometric Identities

Using the cosine identity, the first diagonal entry becomes:

$$
\cos(\alpha+\beta)
$$

Using the sine identity, the second row, first column becomes:

$$
\sin(\alpha+\beta)
$$

The first row, second column becomes:

$$
-\sin(\alpha+\beta)
$$

The second diagonal entry becomes:

$$
\cos(\alpha+\beta)
$$

Therefore:

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos(\alpha+\beta)&-\sin(\alpha+\beta)\\
\sin(\alpha+\beta)&\cos(\alpha+\beta)
\end{pmatrix}
$$

### 6. Verify the Final Result

Recall the definition of a rotation matrix:

$$
R(\theta)=
\begin{pmatrix}
\cos\theta&-\sin\theta\\
\sin\theta&\cos\theta
\end{pmatrix}
$$

Replacing θ with α + β:

$$
R(\alpha+\beta)=
\begin{pmatrix}
\cos(\alpha+\beta)&-\sin(\alpha+\beta)\\
\sin(\alpha+\beta)&\cos(\alpha+\beta)
\end{pmatrix}
$$

Comparing both matrices, we obtain:

$$
\boxed{R(\alpha)R(\beta)=R(\alpha+\beta)}
$$

Thus, the required identity is proven.

### 7. Geometric Explanation

A rotation matrix changes the direction of a vector without changing its length.

When we first rotate a vector by an angle β and then rotate it by an angle α, the total rotation is the sum of these two angles.

Therefore:

- The first rotation changes the direction by β.
- The second rotation adds another rotation of α.
- The final direction is rotated by α + β.
- The length of the vector remains unchanged.

For example, if we rotate a vector by 30° and then by 60°, the total rotation is:

$$
30^\circ+60^\circ=90^\circ
$$

This is exactly equivalent to one rotation of 90°.

### 8. Final Conclusion

We have demonstrated algebraically that multiplying two rotation matrices is equivalent to adding their rotation angles.

The final identity is:

$$
\boxed{R(\alpha)R(\beta)=R(\alpha+\beta)}
$$

Geometrically, this means that two consecutive rotations in the plane produce the same result as one rotation through the sum of their angles.

This exercise demonstrates the consistency between matrix multiplication, trigonometric identities, and geometric rotations.
