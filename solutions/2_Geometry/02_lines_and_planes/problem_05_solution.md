# Exercise 5. Relative Position of Two Lines

## Question

**Given:**

Two lines in $\mathbb{R}^3$:

$$L_1: (x, y, z) = (1, 1, 0) + t(1, 2, 1), \qquad t \in \mathbb{R}$$

$$L_2: (x, y, z) = (2, 0, 1) + s(0, 1, -1), \qquad s \in \mathbb{R}$$

**Required:**

1. Analyze the relative position of $L_1$ and $L_2$.
2. If they intersect, give the intersection point; if not, determine whether they are parallel or skew.
3. Justify the classification.

> **Why this exercise:** Teaches how to distinguish qualitatively different relationships between lines in space.

---

## Solution

### Step 1. Check Whether the Lines Are Parallel

Extract the direction vectors of $L_1$ and $L_2$:

$$d_1 = (1, 2, 1), \qquad d_2 = (0, 1, -1)$$

For $L_1$ and $L_2$ to be parallel, there must exist a scalar $k \in \mathbb{R}$ such that $d_1 = k d_2$. Comparing the first components gives $1 = k \cdot 0 = 0$, which is impossible. Therefore, $d_1$ and $d_2$ are not proportional, so **$L_1$ and $L_2$ are not parallel** (nor coincident).

---

### Step 2. Test for an Intersection Point

Equate the parametric coordinates of $L_1$ and $L_2$ to check whether there exists a pair $(t, s) \in \mathbb{R}^2$ satisfying all three equations simultaneously:

$$1 + t = 2 \qquad (1)$$

$$1 + 2t = s \qquad (2)$$

$$t = 1 - s \qquad (3)$$

From equation $(1)$:

$$t = 2 - 1 = 1$$

Substitute $t = 1$ into equation $(2)$:

$$s = 1 + 2(1) = 3$$

Now test $(t, s) = (1, 3)$ in equation $(3)$:

$$\text{LHS} = t = 1, \qquad \text{RHS} = 1 - s = 1 - 3 = -2$$

Since $1 \neq -2$, equation $(3)$ is contradicted, so the system is inconsistent and **no intersection point exists**.

---

### Step 3. Classification and Justification

In $\mathbb{R}^3$, two lines that neither share a direction vector (not parallel) nor share a common point (non-intersecting) are classified as **skew lines** (they lie in distinct parallel planes without meeting).

---

### Final Answer

- **Classification:** The lines $L_1$ and $L_2$ are **skew**.
- **Intersection point:** None (the coordinate system yields $t = 1$ and $s = 3$, which violates the third equation $1 \neq -2$).
- **Justification:** Their direction vectors $d_1 = (1, 2, 1)$ and $d_2 = (0, 1, -1)$ are not scalar multiples (not parallel), and their parametric equations have no simultaneous solution (non-intersecting).
