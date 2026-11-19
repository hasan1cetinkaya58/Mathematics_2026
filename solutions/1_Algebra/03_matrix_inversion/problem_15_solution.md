# Exercise 15. Two Methods for Solving the Same System

## Question

**Given:**

Consider the linear system $Ax = b$, where:

$$
A = \begin{bmatrix} 2 & 1 \\ 1 & 3 \end{bmatrix}, \qquad b = \begin{bmatrix} 7 \\ 8 \end{bmatrix}
$$

**Required:**

Solve $Ax = b$ in two ways:
1. Using $x = A^{-1}b$.
2. Using Gaussian elimination.

Then:
3. Compare both solutions and the number of essential steps.
4. State which method was simpler in this example.

> **Why this exercise:** Compares two known methods and prepares the student to choose a solution method consciously.

---

## Solution

### Step 1. Method 1 — Solve Using Inverse Matrix

First, we calculate the determinant of $A$:

$$
\det(A) = (2)(3) - (1)(1) = 6 - 1 = 5 \neq 0
$$

Since $\det(A) = 5 \neq 0$, $A$ is invertible. Using the $2 \times 2$ inverse formula:

$$
A^{-1} = \dfrac{1}{\det(A)} \begin{bmatrix} d & -b \\ -c & a \end{bmatrix} = \dfrac{1}{5} \begin{bmatrix} 3 & -1 \\ -1 & 2 \end{bmatrix} = \begin{bmatrix} \dfrac{3}{5} & -\dfrac{1}{5} \\ -\dfrac{1}{5} & \dfrac{2}{5} \end{bmatrix}
$$

Now, we compute $x = A^{-1}b$:

$$
x = \begin{bmatrix} \dfrac{3}{5} & -\dfrac{1}{5} \\ -\dfrac{1}{5} & \dfrac{2}{5} \end{bmatrix} \begin{bmatrix} 7 \\ 8 \end{bmatrix}
$$

Multiplying row by column:

$$
x = \begin{bmatrix} \dfrac{3}{5} \cdot 7 + \left(-\dfrac{1}{5}\right) \cdot 8 \\ \left(-\dfrac{1}{5}\right) \cdot 7 + \dfrac{2}{5} \cdot 8 \end{bmatrix} = \begin{bmatrix} \dfrac{21 - 8}{5} \\ \dfrac{-7 + 16}{5} \end{bmatrix} = \begin{bmatrix} \dfrac{13}{5} \\ \dfrac{9}{5} \end{bmatrix}
$$

Thus, Method 1 gives:

$$
x = \begin{bmatrix} \dfrac{13}{5} \\ \dfrac{9}{5} \end{bmatrix}
$$

---### Step 2. Method 2 — Solve Using Gaussian Elimination

We write the augmented matrix $[A \mid b]$:

$$
\left[\begin{array}{cc|c} 2 & 1 & 7 \\ 1 & 3 & 8 \end{array}\right]
$$

**Essential Step 1 (Swap $R_1$ and $R_2$ to get pivot $1$ in top-left):**

$$
R_1 \leftrightarrow R_2 \implies \left[\begin{array}{cc|c} 1 & 3 & 8 \\ 2 & 1 & 7 \end{array}\right]
$$

**Essential Step 2 (Eliminate the entry below the pivot):**

$$
R_2 \leftarrow R_2 - 2R_1 \implies \left[\begin{array}{cc|c} 1 & 3 & 8 \\ 0 & -5 & -9 \end{array}\right]
$$

**Essential Step 3 (Normalize the second pivot to $1$):**

$$
R_2 \leftarrow -\dfrac{1}{5}R_2 \implies \left[\begin{array}{cc|c} 1 & 3 & 8 \\ 0 & 1 & \dfrac{9}{5} \end{array}\right]
$$

**Essential Step 4 (Back-substitution to eliminate above the second pivot):**

$$
R_1 \leftarrow R_1 - 3R_2
$$

Computing the first row's right-hand side:

$$
8 - 3 \cdot \dfrac{9}{5} = \dfrac{40 - 27}{5} = \dfrac{13}{5}
$$

This gives the reduced row echelon form (RREF):

$$
\left[\begin{array}{cc|c} 1 & 0 & \dfrac{13}{5} \\ 0 & 1 & \dfrac{9}{5} \end{array}\right]
$$

Reading the solution directly from the augmented matrix:

$$
x = \begin{bmatrix} \dfrac{13}{5} \\ \dfrac{9}{5} \end{bmatrix}
$$

---

### Step 3. Comparison of Both Solutions and Essential Steps

1. **Solutions:** Both methods produce the exact same solution vector:

$$
x = \begin{bmatrix} \dfrac{13}{5} \\ \dfrac{9}{5} \end{bmatrix}
$$

2. **Number of essential steps:**
   - **Inverse method ($x = A^{-1}b$):** Requires **3 essential steps**: (1) computing $\det(A)$, (2) forming $A^{-1}$, and (3) multiplying $A^{-1}b$.
   - **Gaussian elimination:** Requires **4 essential row/elimination steps** (row swap, eliminating below pivot, scaling row 2, and eliminating above pivot / back-substitution).

---

### Step 4. Which Method Was Simpler in This Example?

In this $2 \times 2$ example, **using $x = A^{-1}b$ is slightly simpler and more direct** because:
- The $2 \times 2$ inverse formula is immediate and gives a common denominator of $5$ right away.
- It avoids multiple row-operation updates on the augmented matrix and requires one fewer essential step than full row reduction.
- Note: For larger systems or when solving for multiple right-hand side vectors $b$ with the same $A$, Gaussian elimination / LU factorization is generally preferred.

---

### Final Answer

$$
x = \begin{bmatrix} \dfrac{13}{5} \\ \dfrac{9}{5} \end{bmatrix}
$$

- **Both methods agree:** $x_1 = \dfrac{13}{5}$ and $x_2 = \dfrac{9}{5}$.
- **Essential steps:** $3$ steps for $x = A^{-1}b$ vs. $4$ steps for Gaussian elimination.
- **Simpler method here:** Computing $x = A^{-1}b$ is simpler for this single $2 \times 2$ system.
