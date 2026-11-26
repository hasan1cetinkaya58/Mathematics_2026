
# Exercise 6: Projection and Perpendicular Component

## Question

Given the vectors `u=(4,2)` and `v=(1,1)`, find the projection of `u` onto the direction of `v`.

Then calculate the perpendicular component:

`r = u - proj_v(u)`

Verify that:

`r·v = 0`

Finally, explain the geometric meaning of this result.

> **Why this exercise:** shows projection as a decomposition into parallel and perpendicular components.

## Solution

### 1. Calculating the Projection of u onto v

To find the projection of vector `u` onto the direction of vector `v`, we use the vector projection formula:

`proj_v(u) = (u·v / v·v)v`

The given vectors are:

`u=(4,2)`

`v=(1,1)`

First, calculate the dot product of `u` and `v`:

`u·v = 4*1 + 2*1`

`u·v = 4 + 2`

`u·v = 6`

Next, calculate the dot product of `v` with itself:

`v·v = 1*1 + 1*1`

`v·v = 1 + 1`

`v·v = 2`

Now substitute these values into the projection formula:

`proj_v(u) = (6/2)(1,1)`

Simplifying:

`proj_v(u) = 3(1,1)`

Multiplying each component by 3:

`proj_v(u) = (3,3)`

Therefore, the projection of `u` onto `v` is:

`proj_v(u) = (3,3)`

### 2. Calculating the Perpendicular Component

The perpendicular component is obtained by subtracting the projection from the original vector.

The formula is:

`r = u - proj_v(u)`

Substituting the calculated values:

`r = (4,2) - (3,3)`

Subtracting the corresponding components:

`r = (4-3, 2-3)`

Therefore:

`r = (1,-1)`

This is the component of `u` perpendicular to the direction of `v`.

### 3. Verifying Perpendicularity Using the Dot Product

Two vectors are perpendicular if their dot product is equal to zero.

The condition is:

`r·v = 0`

We have calculated:

`r = (1,-1)`

`v = (1,1)`

Now calculate their dot product:

`r·v = 1*1 + (-1)*1`

Simplifying:

`r·v = 1 - 1`

Therefore:

`r·v = 0`

This confirms that the perpendicular component is indeed perpendicular to `v`.

### 4. Geometric Interpretation

The original vector `u` can be decomposed into two components:

- The parallel component is the projection of `u` onto `v`, which is `(3,3)`.
- The perpendicular component is `r=(1,-1)`.

The original vector is reconstructed by adding these two components:

`u = proj_v(u) + r`

Substituting the values:

`u = (3,3) + (1,-1)`

Adding the corresponding components:

`u = (4,2)`

This gives us the original vector.

Geometrically, the projection represents the part of `u` that points along the direction of `v`.

The remaining component is perpendicular to `v`, forming a right angle with it.

Therefore, the original vector is separated into two perpendicular components: one parallel to `v` and one perpendicular to `v`.

## Final Results

**Original vector:**

`u = (4,2)`

**Direction vector:**

`v = (1,1)`

**Projection of u onto v:**

`proj_v(u) = (3,3)`

**Perpendicular component:**

`r = (1,-1)`

**Perpendicularity verification:**

`r·v = 0`

**Reconstruction:**

`u = (3,3) + (1,-1) = (4,2)`

**Conclusion:**

The vector `u` can be decomposed into a parallel component and a perpendicular component relative to `v`.

The projection gives the parallel component, while subtracting it from the original vector gives the perpendicular component.

Both components reconstruct the original vector, and the dot product confirms that they are perpendicular.

The exercise is solved correctly.
