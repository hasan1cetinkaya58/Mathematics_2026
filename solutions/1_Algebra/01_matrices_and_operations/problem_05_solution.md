
# Exercise 5: Matrix Times Vector

## Question

Let

$$
A=
\begin{pmatrix}
2 & -1\\
1 & 3
\end{pmatrix},
\qquad
x=
\begin{pmatrix}
4\\
2
\end{pmatrix}.
$$

Compute $Ax$. Then express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the vector $x$.

## Solution

### 1. Check the Dimensions

Matrix $A$ has dimensions $2 \times 2$, and vector $x$ has dimensions $2 \times 1$.

The number of columns of $A$ is equal to the number of rows of $x$. Therefore, the product $Ax$ is defined and the result has dimensions $2 \times 1$.

### 2. Calculate the Matrix-Vector Product

Multiply each row of matrix $A$ by the column vector $x$.

$$
Ax=
\begin{pmatrix}
2 & -1\\
1 & 3
\end{pmatrix}
\begin{pmatrix}
4\\
2
\end{pmatrix}
$$

The first entry is:

$$
2\cdot4+(-1)\cdot2=8-2=6
$$

The second entry is:

$$
1\cdot4+3\cdot2=4+6=10
$$

Therefore,

$$
\boxed{
Ax=
\begin{pmatrix}
6\\
10
\end{pmatrix}
}
$$

### 3. Express the Result as a Linear Combination of the Columns of A

The columns of matrix $A$ are:

$$
a_1=
\begin{pmatrix}
2\\
1
\end{pmatrix},
\qquad
a_2=
\begin{pmatrix}
-1\\
3
\end{pmatrix}.
$$

The entries of vector $x$ are 4 and 2. These entries become the coefficients of the corresponding columns.

Thus,

$$
Ax=4a_1+2a_2
$$

Substituting the column vectors:

$$
Ax=
4\begin{pmatrix}
2\\
1
\end{pmatrix}
+
2\begin{pmatrix}
-1\\
3
\end{pmatrix}
$$

Multiplying each column by its coefficient:

$$
Ax=
\begin{pmatrix}
8\\
4
\end{pmatrix}
+
\begin{pmatrix}
-2\\
6
\end{pmatrix}
$$


Adding the vectors:



$$
\begin{aligned}
Ax &= 4\begin{pmatrix}2\\1\end{pmatrix}
+ 2\begin{pmatrix}-1\\3\end{pmatrix}\\
&= \begin{pmatrix}8\\4\end{pmatrix}
+ \begin{pmatrix}-2\\6\end{pmatrix}\\
&= \begin{pmatrix}6\\10\end{pmatrix}
\end{aligned}
$$




### 4. Verification

The direct matrix-vector multiplication and the linear combination of the columns give the same result:




$$
\begin{pmatrix}6\\10\end{pmatrix}
=
\begin{pmatrix}6\\10\end{pmatrix}
$$


This verifies the calculation.

## Final Answer

$$
\boxed{
Ax=
\begin{pmatrix}
6\\
10
\end{pmatrix}
}
$$

The linear combination of the columns of $A$ is:

$$
\boxed{Ax=4a_1+2a_2}
$$

This example demonstrates that multiplying a matrix by a vector is equivalent to taking a linear combination of the matrix columns, using the entries of the vector as coefficients.
