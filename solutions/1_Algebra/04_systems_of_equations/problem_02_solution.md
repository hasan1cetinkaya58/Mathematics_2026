# Exercise 2. Gaussian Elimination — One Solution

## Question

**Given:**

Consider the following system of three linear equations in three unknowns:

$$x + y + z = 6$$

$$2x - y + z = 3$$

$$x + 2y - z = 2$$

**Required:**

1. Solve the system using Gaussian elimination.
2. Substitute the resulting values into all three original equations and check consistency.

> **Why this exercise:** Introduces the basic method for solving a system and builds the habit of checking the result.

---

## Solution

### Step 1. Form the Augmented Matrix

We write the augmented matrix $[A \mid b]$ corresponding to the system:

$$\left[\begin{array}{ccc|c} 1 & 1 & 1 & 6 \\ 2 & -1 & 1 & 3 \\ 1 & 2 & -1 & 2 \end{array}\right]$$

---

### Step 2. Forward Elimination (Row Echelon Form)

The top-left entry is already a leading $1$ in Row 1 ($R_1$).

**1. Eliminate below the first pivot ($x$ in $R_2$ and $R_3$):**

We apply $R_2 \leftarrow R_2 - 2R_1$:

$$R_2 - 2R_1 = (2,\ -1,\ 1 \mid 3) - (2,\ 2,\ 2 \mid 12) = (0,\ -3,\ -1 \mid -9)$$

We apply $R_3 \leftarrow R_3 - R_1$:

$$R_3 - R_1 = (1,\ 2,\ -1 \mid 2) - (1,\ 1,\ 1 \mid 6) = (0,\ 1,\ -2 \mid -4)$$

The matrix becomes:

$$\left[\begin{array}{ccc|c} 1 & 1 & 1 & 6 \\ 0 & -3 & -1 & -9 \\ 0 & 1 & -2 & -4 \end{array}\right]$$

**2. Pivot in the second column ($y$):**

Swap $R_2$ and $R_3$ ($R_2 \leftrightarrow R_3$) to get a clean leading $1$ in the second pivot position:

$$\left[\begin{array}{ccc|c} 1 & 1 & 1 & 6 \\ 0 & 1 & -2 & -4 \\ 0 & -3 & -1 & -9 \end{array}\right]$$

Now eliminate below the second pivot by applying $R_3 \leftarrow R_3 + 3R_2$:

$$R_3 + 3R_2 = (0,\ -3,\ -1 \mid -9) + (0,\ 3,\ -6 \mid -12) = (0,\ 0,\ -7 \mid -21)$$

We obtain the upper triangular (row echelon) form:

$$\left[\begin{array}{ccc|c} 1 & 1 & 1 & 6 \\ 0 & 1 & -2 & -4 \\ 0 & 0 & -7 & -21 \end{array}\right]$$

---

### Step 3. Back-Substitution

The row echelon matrix corresponds to the triangular system:

$$x + y + z = 6$$

$$y - 2z = -4$$

$$-7z = -21$$

1. **Solve for $z$ from the third equation:**

$$-7z = -21 \implies z = \dfrac{-21}{-7} = 3$$

2. **Substitute $z = 3$ into the second equation to find $y$:**

$$y - 2(3) = -4 \implies y - 6 = -4 \implies y = 2$$

3. **Substitute $y = 2$ and $z = 3$ into the first equation to find $x$:**

$$x + 2 + 3 = 6 \implies x + 5 = 6 \implies x = 1$$

Thus, the system has a **unique solution** (one solution):

$$(x,\ y,\ z) = (1,\ 2,\ 3)$$

---

### Step 4. Substitute Into All Equations and Check Consistency

We substitute $x = 1$, $y = 2$, and $z = 3$ into each original equation:

- **First equation ($x + y + z = 6$):**

$$1 + 2 + 3 = 6 \quad \text{(Matches } 6 \text{ — consistent)}$$

- **Second equation ($2x - y + z = 3$):**

$$2(1) - 2 + 3 = 2 - 2 + 3 = 3 \quad \text{(Matches } 3 \text{ — consistent)}$$

- **Third equation ($x + 2y - z = 2$):**

$$1 + 2(2) - 3 = 1 + 4 - 3 = 2 \quad \text{(Matches } 2 \text{ — consistent)}$$

All three equations are satisfied simultaneously, confirming that the solution is consistent and unique.

---

### Final Answer

The system has a unique solution:

$$x = 1, \qquad y = 2, \qquad z = 3$$

Written as an ordered triple or column vector:

$$(x,\ y,\ z) = (1,\ 2,\ 3), \qquad \mathbf{x} = \begin{bmatrix} 1 \\ 2 \\ 3 \end{bmatrix}$$

Substituting $(1,\ 2,\ 3)$ into all three equations gives $6 = 6$, $3 = 3$, and $2 = 2$, verifying full consistency.
