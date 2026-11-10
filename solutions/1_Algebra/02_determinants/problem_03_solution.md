
# Exercise 3: Swapping Two Rows

## Question

Given the matrix:

$$
A =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 3 & 1 \\
2 & 1 & 1
\end{pmatrix}
$$

Compute $\det(A)$. Then form a matrix $B$ by swapping the first and second rows of $A$.

First predict $\det(B)$ using a determinant property, and then verify your prediction by calculation.

## Solution

### 1. Calculate the Determinant of A

We are given:

$$
A =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 3 & 1 \\
2 & 1 & 1
\end{pmatrix}
$$

Using Sarrus' rule, the determinant of a 3×3 matrix is the sum of the downward diagonal products minus the sum of the upward diagonal products.

First, calculate the downward diagonal products:

$$
1 \cdot 3 \cdot 1 = 3
$$

$$
2 \cdot 1 \cdot 2 = 4
$$

$$
0 \cdot 0 \cdot 1 = 0
$$

Their sum is:

$$
3+4+0=7
$$

Next, calculate the upward diagonal products:

$$
0 \cdot 3 \cdot 2 = 0
$$

$$
2 \cdot 0 \cdot 1 = 0
$$

$$
1 \cdot 1 \cdot 1 = 1
$$

Their sum is:

$$
0+0+1=1
$$

Therefore:

$$
\det(A)=7-1
$$

$$
\boxed{\det(A)=6}
$$

### 2. Swap the First and Second Rows

We form matrix B by swapping the first and second rows of A.

The new matrix is:

$$
B =
\begin{pmatrix}
0 & 3 & 1 \\
1 & 2 & 0 \\
2 & 1 & 1
\end{pmatrix}
$$

### 3. Predict the New Determinant

One important property of determinants states that swapping two rows of a matrix changes the sign of its determinant.

Therefore:

$$
\det(B)=-\det(A)
$$

Since:

$$
\det(A)=6
$$

Our prediction is:

$$
\boxed{\det(B)=-6}
$$

### 4. Verify the Result Using Sarrus' Rule

Now we calculate the determinant of B directly.

First, calculate the downward diagonal products:

$$
0 \cdot 2 \cdot 1 = 0
$$

$$
3 \cdot 0 \cdot 2 = 0
$$

$$
1 \cdot 1 \cdot 1 = 1
$$

Their sum is:

$$
0+0+1=1
$$

Next, calculate the upward diagonal products:

$$
1 \cdot 2 \cdot 2 = 4
$$

$$
3 \cdot 1 \cdot 1 = 3
$$

$$
0 \cdot 0 \cdot 1 = 0
$$

Their sum is:

$$
4+3+0=7
$$

Subtracting the upward diagonal sum from the downward diagonal sum:

$$
\det(B)=1-7
$$

Therefore:

$$
\boxed{\det(B)=-6}
$$

### 5. Compare the Results

Our calculations give:

$$
\det(A)=6
$$

$$
\det(B)=-6
$$

The direct calculation confirms our prediction.

Swapping the first and second rows changes the determinant from 6 to -6.

### 6. Final Conclusion

We have demonstrated that swapping two rows of a square matrix changes the sign of its determinant but does not change its absolute value.

The relationship is:

$$
\boxed{\det(B)=-\det(A)}
$$

This exercise illustrates an important property of determinants and shows how row operations affect their values.
