
# Exercise 4: Gauss–Jordan Method

## Question

Find \(A^{-1}\) using the Gauss–Jordan method for

$$
A =
\begin{pmatrix}
1 & 2 \\
3 & 5
\end{pmatrix}
$$

Show the augmented matrix \([A \mid I]\) after successive operations and explain why obtaining \(I\) on the left gives the inverse on the right.

## Solution

### Step 1. Construct the Augmented Matrix

First, we write the original matrix \(A\) next to the identity matrix \(I\).

$$
[A \mid I] =
\left[
\begin{array}{cc|cc}
1 & 2 & 1 & 0 \\
3 & 5 & 0 & 1
\end{array}
\right]
$$

The goal is to transform the left side into the identity matrix.

### Step 2. Eliminate the Entry Below the First Pivot

We need to eliminate the number 3 in the second row and first column.

We apply the row operation:

$$
R_2 \rightarrow R_2 - 3R_1
$$

Calculating the new second row:

$$
R_2 =
(3,5,0,1)-3(1,2,1,0)
$$

$$
R_2 =
(3-3,\ 5-6,\ 0-3,\ 1-0)
$$

$$
R_2 = (0,-1,-3,1)
$$

The new augmented matrix becomes:

$$
\left[
\begin{array}{cc|cc}
1 & 2 & 1 & 0 \\
0 & -1 & -3 & 1
\end{array}
\right]
$$

### Step 3. Make the Second Pivot Equal to 1

The second pivot is currently \(-1\). We multiply the entire second row by \(-1\).

We apply:

$$
R_2 \rightarrow -R_2
$$

The new augmented matrix is:

$$
\left[
\begin{array}{cc|cc}
1 & 2 & 1 & 0 \\
0 & 1 & 3 & -1
\end{array}
\right]
$$

Now both pivots are equal to 1.

### Step 4. Eliminate the Entry Above the Second Pivot

We need to eliminate the number 2 in the first row and second column.

We apply the row operation:

$$
R_1 \rightarrow R_1 - 2R_2
$$

Calculating the new first row:

$$
R_1 =
(1,2,1,0)-2(0,1,3,-1)
$$

$$
R_1 =
(1-0,\ 2-2,\ 1-6,\ 0+2)
$$

$$
R_1 = (1,0,-5,2)
$$

The final augmented matrix becomes:

$$
\left[
\begin{array}{cc|cc}
1 & 0 & -5 & 2 \\
0 & 1 & 3 & -1
\end{array}
\right]
$$

### Step 5. Obtain the Inverse Matrix

The left side of the augmented matrix is now the identity matrix \(I\).

$$
\left[
\begin{array}{cc|cc}
1 & 0 & -5 & 2 \\
0 & 1 & 3 & -1
\end{array}
\right]
$$

Since the left side has become \(I\), the right side represents the inverse of the original matrix.

Therefore:

$$
\boxed{
A^{-1} =
\begin{pmatrix}
-5 & 2 \\
3 & -1
\end{pmatrix}
}
$$

### Step 6. Explanation

Each elementary row operation is equivalent to multiplying the matrix by an invertible elementary matrix.

If these operations transform \(A\) into the identity matrix \(I\), the same operations transform \(I\) into \(A^{-1}\).

Mathematically:

$$
EA = I
$$

Therefore:

$$
E = A^{-1}
$$

This explains why obtaining the identity matrix on the left gives the inverse matrix on the right.

### Final Answer

$$
\boxed{
A^{-1} =
\begin{pmatrix}
-5 & 2 \\
3 & -1
\end{pmatrix}
}
$$

The Gauss–Jordan method successfully transforms the augmented matrix \([A \mid I]\) into \([I \mid A^{-1}]\). Therefore, the inverse of the original matrix is obtained.
