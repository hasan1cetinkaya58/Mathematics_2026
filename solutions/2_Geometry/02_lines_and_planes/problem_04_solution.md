# Exercise 4. Plane Through Three Points

## Question

**Given:**

Three points in $\mathbb{R}^3$:

$$A = (1, 0, 0), \qquad B = (0, 1, 0), \qquad C = (0, 0, 1)$$

**Required:**

1. Construct two vectors lying in the plane.
2. Use the cross product to find a normal vector and write the equation of the plane.
3. Check the resulting equation on all three points.

> **Why this exercise:** Connects earlier vector tools with constructing the equation of a plane.

---

## Solution

### Step 1. Construct Two Vectors in the Plane

Form two displacement vectors starting at $A = (1, 0, 0)$:

$$u = \overrightarrow{AB} = B - A = (0 - 1,\ 1 - 0,\ 0 - 0) = (-1, 1, 0)$$

$$v = \overrightarrow{AC} = C - A = (0 - 1,\ 0 - 0,\ 1 - 0) = (-1, 0, 1)$$

Since $u$ and $v$ are not scalar multiples of each other, they span the plane.

---

### Step 2. Compute the Normal Vector and Equation of the Plane

Compute the cross product $n = u \times v$ to obtain a vector perpendicular to both $u$ and $v$:

$$n = (-1, 1, 0) \times (-1, 0, 1) = (1 \cdot 1 - 0 \cdot 0,\ 0 \cdot (-1) - (-1) \cdot 1,\ (-1) \cdot 0 - 1 \cdot (-1)) = (1, 1, 1)$$

Using the point-normal form $n \cdot (X - A) = 0$ with $n = (1, 1, 1)$ and $A = (1, 0, 0)$:

$$1(x - 1) + 1(y - 0) + 1(z - 0) = 0 \implies x + y + z - 1 = 0$$

Thus, the equation of the plane is:

$$x + y + z = 1$$

---

### Step 3. Check the Equation on All Three Points

Substitute each given point into $x + y + z = 1$:

- **At $A = (1, 0, 0)$:** $1 + 0 + 0 = 1$ (satisfied)
- **At $B = (0, 1, 0)$:** $0 + 1 + 0 = 1$ (satisfied)
- **At $C = (0, 0, 1)$:** $0 + 0 + 1 = 1$ (satisfied)

All three points lie on the plane.

---

### Final Answer

- **Two vectors in the plane:** $\overrightarrow{AB} = (-1, 1, 0)$ and $\overrightarrow{AC} = (-1, 0, 1)$
- **Normal vector:** $n = (1, 1, 1)$
- **Equation of the plane:** $x + y + z = 1$ (or $x + y + z - 1 = 0$)
