
# Exercise 11: When Do Matrices Commute?

## Question

Given the matrices:

$$
A = \begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix},
\qquad
B = \begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
$$

Find the conditions on \(a,b,c,d\) under which \(AB=BA\). Describe the general form of all such matrices \(B\).

## Solution

### 1. Identify the Given Matrices

We are given two \(2 \times 2\) matrices:

$$
A = \begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

and

$$
B = \begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
$$

Our goal is to find all values of \(a,b,c,d\) for which:

$$
AB = BA
$$

This means that multiplying the matrices in either order must produce exactly the same result.

### 2. Calculate the Product AB

First, we multiply matrix \(A\) by matrix \(B\):

$$
AB =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
$$

Using row-by-column multiplication:

First row, first column:

$$
1 \cdot a + 1 \cdot c = a+c
$$

First row, second column:

$$
1 \cdot b + 1 \cdot d = b+d
$$

Second row, first column:

$$
0 \cdot a + 1 \cdot c = c
$$

Second row, second column:

$$
0 \cdot b + 1 \cdot d = d
$$

Therefore:

$$
AB =
\begin{pmatrix}
a+c & b+d \\
c & d
\end{pmatrix}
$$

### 3. Calculate the Product BA

Now, we multiply matrix \(B\) by matrix \(A\) in the reverse order:

$$
BA =
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

Using row-by-column multiplication:

First row, first column:

$$
a \cdot 1 + b \cdot 0 = a
$$

First row, second column:

$$
a \cdot 1 + b \cdot 1 = a+b
$$

Second row, first column:

$$
c \cdot 1 + d \cdot 0 = c
$$

Second row, second column:

$$
c \cdot 1 + d \cdot 1 = c+d
$$

Therefore:

$$
BA =
\begin{pmatrix}
a & a+b \\
c & c+d
\end{pmatrix}
$$




### 4. Set AB Equal to BA

For the matrices to commute, their corresponding entries must be equal.

Comparing the corresponding entries of AB and BA gives four equations.

First entry:

$$
a+c=a
$$

Therefore:

$$
c=0
$$

Second entry:

$$
b+d=a+b
$$

Therefore:

$$
d=a
$$

Third entry:

$$
c=c
$$

This equation is always true and gives no additional condition.

Fourth entry:

$$
d=c+d
$$

Therefore:

$$
c=0
$$

The necessary and sufficient conditions are:

$$
c=0,\qquad d=a
$$


### 5. Determine the Conditions

Combining all the equations, we obtain:

$$
\boxed{c=0,\qquad d=a}
$$

There is no restriction on the values of \(a\) and \(b\).

Therefore, \(a\) and \(b\) can be any real numbers.

### 6. Describe the General Form of B

Substituting the conditions \(c=0\) and \(d=a\) into the original matrix \(B\), we obtain:

$$
B =
\begin{pmatrix}
a & b \\
0 & a
\end{pmatrix}
$$

This is the general form of every matrix \(B\) that commutes with matrix \(A\).

### 7. Verify the Result

To verify our result, we substitute the general form of \(B\) into both products.

First:

$$
AB =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
a & b \\
0 & a
\end{pmatrix}
$$

Multiplying the matrices:

$$
AB =
\begin{pmatrix}
a & a+b \\
0 & a
\end{pmatrix}
$$

Now calculate \(BA\):

$$
BA =
\begin{pmatrix}
a & b \\
0 & a
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

Multiplying the matrices:

$$
BA =
\begin{pmatrix}
a & a+b \\
0 & a
\end{pmatrix}
$$

Since both products are identical:

$$
\boxed{AB=BA}
$$

The result is verified.

## Final Answer

The necessary and sufficient conditions for \(AB=BA\) are:

$$
\boxed{c=0,\qquad d=a}
$$

There are no restrictions on \(a\) and \(b\).

Therefore, the general form of all matrices \(B\) that commute with \(A\) is:

$$
\boxed{
B =
\begin{pmatrix}
a & b \\
0 & a
\end{pmatrix}
}
$$

### Conclusion

Matrix multiplication is generally not commutative, meaning that \(AB\) and \(BA\) are not usually equal.

However, this exercise demonstrates that certain matrices can commute when specific conditions are satisfied.

In this case, matrix \(B\) must have zeros in its bottom-left position and equal diagonal entries.

Thus, infinitely many matrices commute with the given matrix \(A\).
