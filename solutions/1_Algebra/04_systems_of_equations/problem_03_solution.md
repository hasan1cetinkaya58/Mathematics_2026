# Exercise 3. Inconsistent System

## Question

**Given:**

Consider the following system of two linear equations in two unknowns:

$$x + 2y = 3$$

$$2x + 4y = 7$$

**Required:**

1. Solve the system or show that it is inconsistent (has no solution).
2. Show how the contradiction appears in the matrix after elimination.
3. Interpret the contradiction in terms of equations.

> **Why this exercise:** Teaches how to recognize that a system has no solution without guessing.

---

## Solution

### Step 1. Form the Augmented Matrix

We write the augmented matrix $[A \mid b]$ for the given system:

$$\left[\begin{array}{cc|c} 1 & 2 & 3 \\ 2 & 4 & 7 \end{array}\right]$$

---

### Step 2. Apply Elimination to the Matrix

We eliminate the entry below the pivot in the first column by applying the row operation $R_2 \leftarrow R_2 - 2R_1$:

$$R_2 - 2R_1 = (2,\ 4 \mid 7) - 2(1,\ 2 \mid 3) = (2,\ 4 \mid 7) - (2,\ 4 \mid 6) = (0,\ 0 \mid 1)$$

After elimination, the matrix becomes:

$$\left[\begin{array}{cc|c} 1 & 2 & 3 \\ 0 & 0 & 1 \end{array}\right]$$

---

### Step 3. Identify the Contradiction in the Matrix and Interpret It as an Equation

Look at the second row of the eliminated matrix:

$$\left[\begin{array}{cc|c} 0 & 0 & 1 \end{array}\right]$$

Translated back into a linear equation, this row represents:

$$0x + 0y = 1 \implies 0 = 1$$

**Interpretation in terms of equations:**
- For any values of $x$ and $y$, the left-hand side $0x + 0y$ is always equal to $0$.
- The right-hand side is $1$, which gives the impossible statement $0 = 1$.
- Geometrically, the two original lines $x + 2y = 3$ and $2x + 4y = 7$ have the same slope ($-\dfrac{1}{2}$) but different $y$-intercepts ($\dfrac{3}{2}$ and $\dfrac{7}{4}$), so they are **parallel and distinct** and never intersect.

Because no pair $(x, y)$ can satisfy $0 = 1$, the system is **inconsistent** and has **no solution**.

---

### Final Answer

The system is **inconsistent** (**no solution**).

- **Matrix after elimination:**

$$\left[\begin{array}{cc|c} 1 & 2 & 3 \\ 0 & 0 & 1 \end{array}\right]$$

- **Contradictory equation from Row 2:**

$$0x + 0y = 1 \implies 0 = 1$$

Since $0 = 1$ is false for all $(x, y)$, there is no solution.
