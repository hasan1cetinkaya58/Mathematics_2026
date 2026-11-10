
# Exercise 9: Area and the Determinant

## Question

The vectors:

$$
u=(3,1),\qquad v=(1,4)
$$

span a parallelogram.

Compute its area using a determinant. Then reverse the order of the vectors and explain what changes in the determinant and what does not change in the area.

## Solution

### 1. Represent the Vectors as a Matrix

We are given two vectors:

$$
u=\begin{pmatrix}3\\1\end{pmatrix},
\qquad
v=\begin{pmatrix}1\\4\end{pmatrix}
$$

To calculate the area of the parallelogram, we place these vectors as the columns of a matrix.

Therefore:

$$
A=
\begin{pmatrix}
3&1\\
1&4
\end{pmatrix}
$$

### 2. Calculate the Determinant

For a 2×2 matrix, the determinant formula is:

$$
\det(A)=ad-bc
$$

Applying the formula to our matrix:

$$
\det(A)=3\cdot4-1\cdot1
$$

Calculating the products:

$$
\det(A)=12-1
$$

Therefore:

$$
\boxed{\det(A)=11}
$$

### 3. Calculate the Area of the Parallelogram

The area of a parallelogram formed by two vectors is the absolute value of the determinant of the matrix containing those vectors as columns.

The formula is:

$$
\text{Area}=|\det(A)|
$$

Substituting our result:

$$
\text{Area}=|11|
$$

Therefore:

$$
\boxed{\text{Area}=11}
$$

The absolute value is used because a geometric area cannot be negative.

### 4. Reverse the Order of the Vectors

Now we reverse the order of the vectors.

Originally, the columns were u and v. We now place v first and u second.

The new matrix is:

$$
B=
\begin{pmatrix}
1&3\\
4&1
\end{pmatrix}
$$

### 5. Calculate the New Determinant

Using the 2×2 determinant formula:

$$
\det(B)=1\cdot1-3\cdot4
$$

Calculating the products:

$$
\det(B)=1-12
$$

Therefore:

$$
\boxed{\det(B)=-11}
$$

### 6. Compare the Determinants and Areas

The original determinant was:

$$
\det(A)=11
$$

After reversing the vectors:

$$
\det(B)=-11
$$

We can observe that:

$$
\det(B)=-\det(A)
$$

Swapping two columns changes the sign of the determinant.

However, the area is calculated using the absolute value.

For the original matrix:

$$
\text{Area}(A)=|11|=11
$$

For the new matrix:

$$
\text{Area}(B)=|-11|=11
$$

Therefore:

$$
\boxed{\text{Area}(A)=\text{Area}(B)=11}
$$

### 7. Geometric Explanation

The determinant represents the signed area of the parallelogram.

Its sign indicates the orientation of the ordered pair of vectors.

When we reverse the order of the vectors:

- The orientation changes.
- The sign of the determinant changes.
- The absolute value of the determinant remains the same.
- The geometric area does not change.

Therefore, reversing the vectors changes the orientation but does not change the size of the parallelogram.

### 8. Final Conclusion

The determinant of the original matrix is:

$$
\boxed{\det(A)=11}
$$

After reversing the order of the vectors:

$$
\boxed{\det(B)=-11}
$$

The area in both cases is:

$$
\boxed{\text{Area}=11}
$$

This exercise demonstrates that the determinant gives a signed geometric area, while its absolute value gives the actual area of the parallelogram.
