# Exercise 6. A System with a Parameter — Which Cases Actually Occur?

## Question

**Given:**

Consider the linear system in $x$ and $y$ depending on the parameter $a \in \mathbb{R}$:

$$x + y = 2$$

$$ax + ay = 4$$

**Required:**

1. Analyze the system depending on the parameter $a$.
2. Among the three possibilities — **exactly one solution**, **infinitely many solutions**, and **no solution** — determine which actually occur and for which values of $a$.
3. If any case cannot occur, explain why.

> **Why this exercise:** Teaches how to analyze a parameter without assuming in advance that all theoretically possible cases must occur in a specific system.

---

## Solution

### Step 1. Set Up the Augmented Matrix and Apply Elimination

We write the augmented matrix $[A \mid b]$ for the system:

$$\left[\begin{array}{cc|c} 1 & 1 & 2 \\ a & a & 4 \end{array}\right]$$

To eliminate the entry in row 2, column 1, we apply the row operation $R_2 \leftarrow R_2 - aR_1$:

$$R_2 - aR_1 = (a,\ a \mid 4) - a(1,\ 1 \mid 2) = (0,\ 0 \mid 4 - 2a)$$

Thus, the eliminated augmented matrix is:

$$\left[\begin{array}{cc|c} 1 & 1 & 2 \\ 0 & 0 & 4 - 2a \end{array}\right]$$

---

### Step 2. Analyze the Cases for the Parameter $a$

Look closely at the coefficient matrix after elimination:

$$A_{\text{elim}} = \begin{bmatrix} 1 & 1 \\ 0 & 0 \end{bmatrix}$$

Notice that the second row of the coefficient matrix is **identically zero** $(0,\ 0)$ for **every** real value of $a$. Therefore, the coefficient matrix always has at most **1 pivot** (in column 1), leaving $y$ as a **free variable** whenever the system is consistent.

Now examine the second row of the augmented matrix, which corresponds to the equation:

$$0x + 0y = 4 - 2a$$

1. **Case 1: No Solution (Inconsistent System)**

   For $0x + 0y = 4 - 2a$ to have no solution, the left-hand side must be $0$ while the right-hand side is nonzero:

   $$4 - 2a \neq 0 \implies a \neq 2$$

   When $a \neq 2$, the second row becomes $0 = c$ with $c = 4 - 2a \neq 0$, which is a contradiction. Hence, for **all $a \neq 2$**, the system has **no solution**.

2. **Case 2: Infinitely Many Solutions (Consistent with a Free Variable)**

   For the second row to become $0 = 0$ (consistent), we need:

   $$4 - 2a = 0 \implies a = 2$$

   When $a = 2$, the matrix becomes:

   $$\left[\begin{array}{cc|c} 1 & 1 & 2 \\ 0 & 0 & 0 \end{array}\right]$$

   Both equations reduce to the single line $x + y = 2$. Setting $y = t$ ($t \in \mathbb{R}$) gives $x = 2 - t$. Thus, for **$a = 2$**, the system has **infinitely many solutions**:

   $$(x,\ y) = (2 - t,\ t), \qquad t \in \mathbb{R}$$

3. **Case 3: Exactly One Solution (Unique Solution) — Cannot Occur**

   **Exactly one solution is impossible for any value of $a$.**

   *Why it cannot occur:* In the original system, the second equation $ax + ay = 4$ is a scalar multiple of the left-hand side of the first equation $x + y = 2$ (specifically, $a(x + y) = 4$). Because the rows of the coefficient matrix $A = \begin{bmatrix} 1 & 1 \\ a & a \end{bmatrix}$ are linearly dependent ($\det(A) = a \cdot 1 - 1 \cdot a = 0$ for all $a$), the two lines are either **parallel and distinct** (no intersection, for $a \neq 2$) or **coincident / the exact same line** (infinitely many intersection points, for $a = 2$). Two distinct or overlapping lines in $\mathbb{R}^2$ can never intersect at a single unique point.

---

### Final Answer

Among the three theoretical cases, **only two occur**:

- **No solution:** For all **$a \neq 2$** (gives the contradiction $0 = 4 - 2a \neq 0$).
- **Infinitely many solutions:** For **$a = 2$** (gives $0 = 0$, with solution $(x,\ y) = (2 - t,\ t)$ for $t \in \mathbb{R}$).
- **Exactly one solution:** **Does not occur for any $a$**, because $\det(A) = 0$ for every $a \in \mathbb{R}$ (the rows of $A$ are linearly dependent, so the equations represent parallel or identical lines, never lines intersecting at a single point).
