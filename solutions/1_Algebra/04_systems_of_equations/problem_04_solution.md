# Exercise 4. Infinitely Many Solutions

## Question

**Given:**

Consider the following system of three linear equations in three unknowns:

$$x + y + z = 2$$

$$2x + 2y + 2z = 4$$

$$x - y + z = 0$$

**Required:**

1. Solve the system and express the solution in parametric form.
2. Identify a free variable.
3. Choose one parameter value and check that the resulting point satisfies all three original equations.

> **Why this exercise:** Shows the case of multiple solutions and teaches a simple parametric description.

---

## Solution

### Step 1. Form the Augmented Matrix

We write the augmented matrix $[A \mid b]$ corresponding to the given system:

$$\left[\begin{array}{ccc|c} 1 & 1 & 1 & 2 \\ 2 & 2 & 2 & 4 \\ 1 & -1 & 1 & 0 \end{array}\right]$$

---

### Step 2. Forward Elimination (Row Echelon Form)

The top-left pivot in Row 1 ($R_1$) is already $1$.

**1. Eliminate below the first pivot ($x$ in $R_2$ and $R_3$):**

Apply $R_2 \leftarrow R_2 - 2R_1$:

$$R_2 - 2R_1 = (2,\ 2,\ 2 \mid 4) - 2(1,\ 1,\ 1 \mid 2) = (0,\ 0,\ 0 \mid 0)$$

Apply $R_3 \leftarrow R_3 - R_1$:

$$R_3 - R_1 = (1,\ -1,\ 1 \mid 0) - (1,\ 1,\ 1 \mid 2) = (0,\ -2,\ 0 \mid -2)$$

The matrix becomes:

$$\left[\begin{array}{ccc|c} 1 & 1 & 1 & 2 \\ 0 & 0 & 0 & 0 \\ 0 & -2 & 0 & -2 \end{array}\right]$$

**2. Swap $R_2$ and $R_3$ ($R_2 \leftrightarrow R_3$) to move the zero row to the bottom and place a nonzero pivot in column 2:**

$$\left[\begin{array}{ccc|c} 1 & 1 & 1 & 2 \\ 0 & -2 & 0 & -2 \\ 0 & 0 & 0 & 0 \end{array}\right]$$

Normalize Row 2 by applying $R_2 \leftarrow -\dfrac{1}{2}R_2$:

$$\left[\begin{array}{ccc|c} 1 & 1 & 1 & 2 \\ 0 & 1 & 0 & 1 \\ 0 & 0 & 0 & 0 \end{array}\right]$$

There is no pivot in the third column ($z$), and the third row is entirely zeros ($0 = 0$), which means the system is consistent and has **infinitely many solutions**.

---

### Step 3. Identify the Free Variable and Write the Parametric Solution

From the row echelon matrix above, we read the equations:

$$y = 1$$

$$x + y + z = 2$$

- **Pivot variables:** $x$ and $y$ (corresponding to columns $1$ and $2$).
- **Free variable:** $z$ (corresponding to column $3$, which has no pivot).

Let $z = t$, where $t \in \mathbb{R}$ is a free parameter.

Substitute $y = 1$ and $z = t$ into $x + y + z = 2$:

$$x + 1 + t = 2 \implies x = 1 - t$$

Thus, the general solution in parametric form is:

$$x = 1 - t, \qquad y = 1, \qquad z = t \qquad (t \in \mathbb{R})$$

Or as a vector:

$$\begin{bmatrix} x \\ y \\ z \end{bmatrix} = \begin{bmatrix} 1 - t \\ 1 \\ t \end{bmatrix} = \begin{bmatrix} 1 \\ 1 \\ 0 \end{bmatrix} + t \begin{bmatrix} -1 \\ 0 \\ 1 \end{bmatrix}, \qquad t \in \mathbb{R}$$

---

### Step 4. Check a Chosen Parameter Value in All Original Equations

Choose the parameter value $t = 2$. Substituting $t = 2$ into the parametric formulas gives the point:

$$x = 1 - 2 = -1, \qquad y = 1, \qquad z = 2 \implies (x,\ y,\ z) = (-1,\ 1,\ 2)$$

Now we substitute $(x,\ y,\ z) = (-1,\ 1,\ 2)$ into all three original equations:

- **First equation ($x + y + z = 2$):**

$$-1 + 1 + 2 = 2 \quad \text{(Matches } 2 \text{ — satisfied)}$$

- **Second equation ($2x + 2y + 2z = 4$):**

$$2(-1) + 2(1) + 2(2) = -2 + 2 + 4 = 4 \quad \text{(Matches } 4 \text{ — satisfied)}$$

- **Third equation ($x - y + z = 0$):**

$$-1 - 1 + 2 = 0 \quad \text{(Matches } 0 \text{ — satisfied)}$$

All three equations hold, confirming that $(-1,\ 1,\ 2)$ is a valid solution.

---

### Final Answer

The system has **infinitely many solutions**.

- **Free variable:** $z = t$ ($t \in \mathbb{R}$).
- **Parametric solution:**

$$x = 1 - t, \qquad y = 1, \qquad z = t \qquad (t \in \mathbb{R})$$

- **Sample check for $t = 2$:** The point $(x,\ y,\ z) = (-1,\ 1,\ 2)$ satisfies $-1 + 1 + 2 = 2$, $2(-1) + 2(1) + 2(2) = 4$, and $-1 - 1 + 2 = 0$.
