
# Exercise 2: Determinant of a 3×3 Matrix

## Question

Given the matrix:

$$
A=
\begin{pmatrix}
1&2&-1\\
0&3&4\\
2&1&5
\end{pmatrix}
$$

Compute the determinant using Sarrus' rule. Then perform one simple check using a property of determinants.

## Solution

### 1. Recall Sarrus' Rule

For a 3×3 matrix:

$$
A=
\begin{pmatrix}
a&b&c\\
d&e&f\\
g&h&i
\end{pmatrix}
$$

Sarrus' rule states that the determinant is:

$$
\det(A)=aei+bfg+cdh-ceg-bdi-afh
$$

We add the products of the three downward diagonals and subtract the products of the three upward diagonals.

### 2. Apply Sarrus' Rule

We are given:

$$
A=
\begin{pmatrix}
1&2&-1\\
0&3&4\\
2&1&5
\end{pmatrix}
$$

First, calculate the products of the downward diagonals:

$$
1\cdot3\cdot5=15
$$

$$
2\cdot4\cdot2=16
$$

$$
(-1)\cdot0\cdot1=0
$$

Adding these products:

$$
15+16+0=31
$$

Next, calculate the products of the upward diagonals:

$$
(-1)\cdot3\cdot2=-6
$$

$$
2\cdot0\cdot5=0
$$

$$
1\cdot4\cdot1=4
$$

Adding these products:

$$
-6+0+4=-2
$$

Now, subtract the sum of the upward diagonal products from the sum of the downward diagonal products:

$$
\det(A)=31-(-2)
$$

Therefore:

$$
\boxed{\det(A)=33}
$$

### 3. Check the Result Using a Determinant Property

We can check our result using the row operation property of determinants.

Adding a multiple of one row to another row does not change the determinant.

Apply the following operation:

$$
R_3\rightarrow R_3-2R_1
$$

The original matrix is:

$$
\begin{pmatrix}
1&2&-1\\
0&3&4\\
2&1&5
\end{pmatrix}
$$

The new third row becomes:

$$
(2,1,5)-2(1,2,-1)
$$

$$
=(0,-3,7)
$$

Therefore, the transformed matrix is:

$$
A'=
\begin{pmatrix}
1&2&-1\\
0&3&4\\
0&-3&7
\end{pmatrix}
$$

Since this row operation does not change the determinant:

$$
\det(A')=\det(A)
$$

Expanding along the first column:

$$
\det(A')=
1\cdot
\begin{vmatrix}
3&4\\
-3&7
\end{vmatrix}
$$

Calculating the 2×2 determinant:

$$
\det(A')=1(3\cdot7-4(-3))
$$

$$
=21+12
$$

Therefore:

$$
\boxed{\det(A')=33}
$$

The result agrees with our calculation using Sarrus' rule.

### 4. Final Conclusion

Using Sarrus' rule, we obtained:

$$
\boxed{\det(A)=33}
$$

We also checked the result using the determinant property that adding a multiple of one row to another row does not change the determinant.

Both calculations give the same result.

Therefore, the determinant of the given matrix is:

$$
\boxed{33}
$$

The determinant is non-zero, so the matrix is also invertible.
