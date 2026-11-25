
## Exercise 2: Distance as the Length of a Vector

### Question

Given the points:

$$
A=(1,2,3), \qquad B=(4,-2,6)
$$

1. Construct the vector \(\overrightarrow{AB}\).
2. Compute its length.
3. Compute the distance between the points using the coordinate formula.
4. Explain why both calculations give the same result.

---

### Solution

**1. Constructing the Vector \(\overrightarrow{AB}\)**

To find the vector from point A to point B, we subtract the coordinates of A from the coordinates of B.

The formula is:

$$
\overrightarrow{AB}=B-A
$$

Substituting the given coordinates:

$$
\overrightarrow{AB}=(4,-2,6)-(1,2,3)
$$

Subtracting the corresponding components:

$$
=(4-1,\,-2-2,\,6-3)
$$

Therefore:

$$
\boxed{\overrightarrow{AB}=(3,-4,3)}
$$

**2. Computing the Length of the Vector**

The length (magnitude) of a vector in \(\mathbb{R}^3\) is calculated using the Euclidean norm formula:

$$
\|v\|=\sqrt{x^2+y^2+z^2}
$$

We substitute the components of \(\overrightarrow{AB}=(3,-4,3)\):

$$
\|\overrightarrow{AB}\|
=\sqrt{3^2+(-4)^2+3^2}
$$

Squaring each component:

$$
=\sqrt{9+16+9}
$$

$$
=\sqrt{34}
$$

Therefore:

$$
\boxed{\|\overrightarrow{AB}\|=\sqrt{34}}
$$

**3. Computing the Distance Using the Coordinate Formula**

The distance between two points in three-dimensional space is calculated using:

$$
d(A,B)=
\sqrt{(x_B-x_A)^2+(y_B-y_A)^2+(z_B-z_A)^2}
$$

Substituting the coordinates of A and B:

$$
d(A,B)=
\sqrt{(4-1)^2+(-2-2)^2+(6-3)^2}
$$

Simplifying:

$$
=\sqrt{3^2+(-4)^2+3^2}
$$

$$
=\sqrt{9+16+9}
$$

$$
\boxed{d(A,B)=\sqrt{34}}
$$

**4. Why Do Both Calculations Give the Same Result?**

Both calculations give the same result because the distance between two points is defined as the length of the vector connecting them.

The vector \(\overrightarrow{AB}\) represents the displacement from point A to point B.

When we calculate its length, we measure the straight-line distance between these two points.

In mathematical terms:

$$
\overrightarrow{AB}=B-A
$$

The distance is the magnitude of this difference vector:

$$
d(A,B)=\|B-A\|
$$

Therefore, both methods use exactly the same coordinate differences and the same Euclidean length formula.

---

### Final Results

$$
\boxed{\overrightarrow{AB}=(3,-4,3)}
$$

$$
\boxed{\|\overrightarrow{AB}\|=\sqrt{34}}
$$

$$
\boxed{d(A,B)=\sqrt{34}\approx 5.83}
$$

**Conclusion:** The distance between two points is equal to the length of the vector connecting them. The coordinate distance formula comes directly from the Euclidean norm of the difference vector.
