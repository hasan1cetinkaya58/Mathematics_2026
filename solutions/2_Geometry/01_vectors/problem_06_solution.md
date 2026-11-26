# Exercise 6: Projection and Perpendicular Component

## Question

Given the vectors $u=(4,2)$ and $v=(1,1)$, find the projection of $u$ onto the direction of $v$.

Then calculate the perpendicular component:

$$r = u - \text{proj}_v(u)$$

Verify that:

$$r \cdot v = 0$$

Finally, explain the geometric meaning of this result.

> **Why this exercise:** Shows projection as a decomposition into parallel and perpendicular components.

## Solution

### 1. Calculating the Projection of $u$ onto $v$

To find the projection of $u$ onto the direction of $v$, we use the vector projection formula:

$$\text{proj}_v(u) = \left(\frac{u \cdot v}{v \cdot v}\right)v$$

Given $u=(4,2)$ and $v=(1,1)$, compute the dot products:

$$u \cdot v = 4 \cdot 1 + 2 \cdot 1 = 4 + 2 = 6$$

$$v \cdot v = 1 \cdot 1 + 1 \cdot 1 = 1 + 1 = 2$$

Substitute these values into the projection formula:

$$\text{proj}_v(u) = \frac{6}{2}(1,1) = 3(1,1) = (3,3)$$

### 2. Calculating the Perpendicular Component

Subtract the projection from the original vector:

$$r = u - \text{proj}_v(u) = (4,2) - (3,3) = (4-3,\ 2-3) = (1,-1)$$

### 3. Verifying Perpendicularity Using the Dot Product

Compute the dot product of $r = (1,-1)$ and $v = (1,1)$:

$$r \cdot v = 1 \cdot 1 + (-1) \cdot 1 = 1 - 1 = 0$$

Since $r \cdot v = 0$, the component $r$ is perpendicular to $v$.

### 4. Geometric Interpretation

The original vector $u$ is decomposed into two orthogonal components:

$$u = \text{proj}_v(u) + r = (3,3) + (1,-1) = (4,2)$$

Geometrically, $\text{proj}_v(u) = (3,3)$ represents the shadow (parallel component) of $u$ along the direction of $v$, while $r = (1,-1)$ is the orthogonal residual perpendicular to $v$. Together, they form a right triangle with $u$ as the hypotenuse.

## Final Results

- **Original vector:** $u = (4,2)$
- **Direction vector:** $v = (1,1)$
- **Projection of $u$ onto $v$:** $\text{proj}_v(u) = (3,3)$
- **Perpendicular component:** $r = (1,-1)$
- **Perpendicularity check:** $r \cdot v = 0$
- **Reconstruction:** $u = (3,3) + (1,-1) = (4,2)$

**Conclusion:** The vector $u$ is decomposed into a component parallel to $v$ and a component perpendicular to $v$, which sum back to $u$.
