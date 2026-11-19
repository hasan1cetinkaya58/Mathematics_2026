# Exercise 8. Two Systems with the Same Coefficient Matrix

## Question

**Given:**

Consider the following two systems of linear equations sharing the same coefficient matrix:

**System 1:**

$$2x + y = 5$$

$$x - y = 1$$

**System 2:**

$$2x + y = 1$$

$$x - y = 4$$

**Required:**

1. Solve both systems by Gaussian elimination.
2. Compare the successive elimination steps.
3. Explain which part of the calculation is the same in both cases and why.

> **Why this exercise:** Shows the role of the coefficient matrix independently of the right-hand side.

---

## Solution

### Step 1. Solve System 1 by Elimination

We write the augmented matrix $[A \mid b_1]$ for System 1:

$$\left[\begin{array}{cc|c} 2 & 1 & 5 \\ 1 & -1 & 1 \end{array}\right]$$

**1. Eliminate $x$ in Row 2 using $R_2 \leftarrow R_2 - \dfrac{1}{2}R_1$:**

$$R_2 - \dfrac{1}{2}R_1 = (1,\ -1 \mid 1) - \dfrac{1}{2}(2,\ 1 \mid 5) = \left(0,\ -\dfrac{3}{2} \;\middle|\; -\dfrac{3}{2}\right)$$

The row echelon form is:

$$\left[\begin{array}{cc|c} 2 & 1 & 5 \\ 0 & -\dfrac{3}{2} & -\dfrac{3}{2} \end{array}\right]$$

**2. Back-substitution:**

From Row 2:

$$-\dfrac{3}{2}y = -\dfrac{3}{2} \implies y = 1$$

Substitute $y = 1$ into Row 1 ($2x + y = 5$):

$$2x + 1 = 5 \implies 2x = 4 \implies x = 2$$

Thus, the solution to System 1 is $(x,\ y) = (2,\ 1)$.

---

### Step 2. Solve System 2 by Elimination

We write the augmented matrix $[A \mid b_2]$ for System 2:

$$\left[\begin{array}{cc|c} 2 & 1 & 1 \\ 1 & -1 & 4 \end{array}\right]$$

**1. Eliminate $x$ in Row 2 using $R_2 \leftarrow R_2 - \dfrac{1}{2}R_1$:**

$$R_2 - \dfrac{1}{2}R_1 = (1,\ -1 \mid 4) - \dfrac{1}{2}(2,\ 1 \mid 1) = \left(0,\ -\dfrac{3}{2} \;\middle|\; \dfrac{7}{2}\right)$$

The row echelon form is:

$$\left[\begin{array}{cc|c} 2 & 1 & 1 \\ 0 & -\dfrac{3}{2} & \dfrac{7}{2} \end{array}\right]$$

**2. Back-substitution:**

From Row 2:

$$-\dfrac{3}{2}y = \dfrac{7}{2} \implies y = -\dfrac{7}{3}$$

Substitute $y = -\dfrac{7}{3}$ into Row 1 ($2x + y = 1$):

$$2x - \dfrac{7}{3} = 1 \implies 2x = \dfrac{10}{3} \implies x = \dfrac{5}{3}$$

Thus, the solution to System 2 is $(x,\ y) = \left(\dfrac{5}{3},\ -\dfrac{7}{3}\right)$.

---

### Step 3. Compare the Elimination Steps

- **What is the same:** Both systems share the exact same coefficient matrix $A = \begin{bmatrix} 2 & 1 \\ 1 & -1 \end{bmatrix}$. Consequently, the **pivots**, the **multiplier** ($m = \dfrac{1}{2}$), the **row operation** ($R_2 \leftarrow R_2 - \dfrac{1}{2}R_1$), and the resulting **upper triangular coefficient block** $\begin{bmatrix} 2 & 1 \\ 0 & -\frac{3}{2} \end{bmatrix}$ are identical in both cases.
- **Why:** Elimination multipliers depend solely on the entries of the coefficient matrix $A$ to create zeros below the pivots; the right-hand side vector $b$ only transforms alongside $A$ without affecting the choice of row operations.

---

### Final Answer

- **System 1 solution:** $(x,\ y) = (2,\ 1)$
- **System 2 solution:** $(x,\ y) = \left(\dfrac{5}{3},\ -\dfrac{7}{3}\right)$
- **Comparison:** The row operations ($R_2 \leftarrow R_2 - \dfrac{1}{2}R_1$), multipliers, pivots, and reduced coefficient matrix $\begin{bmatrix} 2 & 1 \\ 0 & -\frac{3}{2} \end{bmatrix}$ are identical because both systems have the same coefficient matrix $A$, which alone determines the elimination steps.
