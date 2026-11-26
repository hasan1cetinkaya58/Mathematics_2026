# Exercise 3. Plane Through a Point with a Given Normal Vector

## Question

**Given:**

A point $P = (1, -2, 3)$ and a normal vector $n = (2, 1, -1)$ in $\mathbb{R}^3$.

**Required:**

1. Find the equation of the plane through $P$ perpendicular to $n$.
2. Check the result by substituting the point $P$.
3. Explain the role of the normal vector.

> **Why this exercise:** Shows the basic construction of a plane from a point and a normal vector.

---

## Solution

### Step 1. Construct the Equation of the Plane

A point $X = (x, y, z)$ lies on the plane through $P = (1, -2, 3)$ with normal vector $n = (2, 1, -1)$ if and only if the displacement vector $\overrightarrow{PX} = X - P$ is orthogonal to $n$:

$$n \cdot (X - P) = 0$$

Substituting the coordinates of $P$ and $n$:

$$2(x - 1) + 1(y - (-2)) - 1(z - 3) = 0$$

Expanding and simplifying:

$$2x - 2 + y + 2 - z + 3 = 0 \implies 2x + y - z + 3 = 0$$

Thus, the general equation of the plane is:

$$2x + y - z + 3 = 0 \quad (\text{or } 2x + y - z = -3)$$

---

### Step 2. Check the Result at $P = (1, -2, 3)$

Substitute $(x, y, z) = (1, -2, 3)$ into $2x + y - z + 3 = 0$:

$$2(1) + (-2) - 3 + 3 = 2 - 2 - 3 + 3 = 0 \quad (\text{satisfied})$$

The point $P$ satisfies the equation.

---

### Step 3. Role of the Normal Vector

The normal vector $n = (2, 1, -1)$ uniquely fixes the **orientation (tilt)** of the plane in $\mathbb{R}^3$ by defining the direction perpendicular to every vector lying within the plane. Its components appear directly as the coefficients $(A, B, C)$ in the general plane equation $Ax + By + Cz + D = 0$, while the point $P$ fixes the specific parallel shift $D$.

---

### Final Answer

- **Equation of the plane:** $2x + y - z + 3 = 0$
- **Verification at $P = (1, -2, 3)$:** $2(1) + (-2) - 3 + 3 = 0$
- **Role of $n$:** Determines the orientation of the plane by being orthogonal to all vectors in the plane, supplying the coefficients of $x$, $y$, and $z$.
