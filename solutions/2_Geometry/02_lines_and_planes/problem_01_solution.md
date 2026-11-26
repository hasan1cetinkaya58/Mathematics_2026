# Exercise 1. Line Through Two Points

## Question

**Given:**

Two points in $\mathbb{R}^2$:

$$A = (1, 2), \qquad B = (4, -1)$$

**Required:**

1. Find the equation of the line through $A$ and $B$ in parametric and general form.
2. Identify a direction vector and an example of a normal vector.
3. Check that both points satisfy the equation obtained.

> **Why this exercise:** Teaches how to move between equivalent descriptions of a line and connect them with the appropriate vectors.

---

## Solution

### Step 1. Direction Vector and Parametric Form

A direction vector $d$ is given by the displacement vector from $A$ to $B$:

$$d = \overrightarrow{AB} = B - A = (4 - 1,\ -1 - 2) = (3, -3)$$

Using point $A = (1, 2)$ and direction vector $d = (3, -3)$, the vector parametric equation of the line is:

$$(x, y) = (1, 2) + t(3, -3), \qquad t \in \mathbb{R}$$

Equivalently, in component (scalar parametric) form:

$$x = 1 + 3t, \qquad y = 2 - 3t, \qquad t \in \mathbb{R}$$

---

### Step 2. Normal Vector and General Form

A normal vector $n = (n_1, n_2)$ must be orthogonal to $d = (3, -3)$, meaning $n \cdot d = 0$. Choosing $n = (1, 1)$ satisfies:

$$n \cdot d = 1 \cdot 3 + 1 \cdot (-3) = 3 - 3 = 0$$

Using the point-normal equation $n \cdot ((x, y) - A) = 0$ with $n = (1, 1)$ and $A = (1, 2)$:

$$1(x - 1) + 1(y - 2) = 0 \implies x + y - 3 = 0$$

Thus, the general form of the line is:

$$x + y - 3 = 0$$

---

### Step 3. Verification of Both Points

Substitute the coordinates of $A$ and $B$ into the general equation $x + y - 3 = 0$:

- **At $A = (1, 2)$:**

$$1 + 2 - 3 = 0 \quad (\text{satisfied})$$

- **At $B = (4, -1)$:**

$$4 + (-1) - 3 = 0 \quad (\text{satisfied})$$

Both points lie on the line.

---

### Final Answer

- **Parametric form:** $x = 1 + 3t,\ y = 2 - 3t$ ($t \in \mathbb{R}$)
- **General form:** $x + y - 3 = 0$
- **Direction vector:** $d = (3, -3)$ (or $(1, -1)$)
- **Normal vector:** $n = (1, 1)$
