## Exercise 10: Triangle Area from Vectors

### Question

Given the points:

$$
A=(0,0,0)
$$

$$
B=(2,1,0)
$$

$$
C=(1,3,2)
$$

1. Construct the vectors $\overrightarrow{AB}$ and $\overrightarrow{AC}$.
2. Compute the area of the parallelogram using the cross product.
3. Find the area of the triangle.
4. Explain why the factor $\frac{1}{2}$ is used.

---

### Solution

**1. Constructing the Vectors AB and AC**

To construct a vector between two points, we subtract the coordinates of the starting point from the coordinates of the ending point.

The formula is:

$$
\overrightarrow{AB}=B-A
$$

Substituting the coordinates:

$$
\overrightarrow{AB}=(2,1,0)-(0,0,0)
$$

Therefore:

$$
\boxed{\overrightarrow{AB}=(2,1,0)}
$$

Now construct the second vector:

$$
\overrightarrow{AC}=C-A
$$

Substituting the coordinates:

$$
\overrightarrow{AC}=(1,3,2)-(0,0,0)
$$

Therefore:

$$
\boxed{\overrightarrow{AC}=(1,3,2)}
$$

**2. Computing the Area of the Parallelogram Using the Cross Product**

The area of a parallelogram formed by two vectors is equal to the length of their cross product.

The formula is:

$$
P=\|\overrightarrow{AB}\times\overrightarrow{AC}\|
$$

First, calculate the cross product.

We have:

$$
\overrightarrow{AB}=(2,1,0)
$$

$$
\overrightarrow{AC}=(1,3,2)
$$

Using the cross product formula:

$$
\overrightarrow{AB}\times\overrightarrow{AC}
$$

$$
=(1\cdot2-0\cdot3,\;
0\cdot1-2\cdot2,\;
2\cdot3-1\cdot1)
$$

Calculating each component:

$$
=(2-0,\;0-4,\;6-1)
$$

Therefore:

$$
\boxed{\overrightarrow{AB}\times\overrightarrow{AC}=(2,-4,5)}
$$

Now calculate the length of the cross product:

$$
P=\sqrt{2^2+(-4)^2+5^2}
$$

$$
=\sqrt{4+16+25}
$$

$$
=\sqrt{45}
$$

Therefore, the area of the parallelogram is:

$$
\boxed{P=3\sqrt{5}}
$$

**3. Finding the Area of the Triangle**

The triangle formed by points A, B, and C occupies exactly half of the parallelogram formed by the same two vectors.

Therefore, the area of the triangle is:

$$
T=\frac{1}{2}P
$$

Substituting the parallelogram area:

$$
T=\frac{1}{2}\cdot3\sqrt{5}
$$

Therefore:

$$
\boxed{T=\frac{3\sqrt{5}}{2}}
$$

The approximate numerical value is:

$$
\boxed{T\approx3.354}
$$

**4. Geometric Explanation of the Factor 1/2**

The two vectors $\overrightarrow{AB}$ and $\overrightarrow{AC}$ form two adjacent sides of a parallelogram.

The diagonal of this parallelogram divides it into two triangles of equal area.

Our triangle ABC is one of these two triangles.

Therefore, its area is exactly half of the parallelogram area.

This explains why we multiply the cross product length by $\frac{1}{2}$.

Geometrically, the relationship is:

$$
T=\frac{1}{2}\times P
$$

---

### Final Results

First vector:

$$
\boxed{\overrightarrow{AB}=(2,1,0)}
$$

Second vector:

$$
\boxed{\overrightarrow{AC}=(1,3,2)}
$$

Cross product:

$$
\boxed{\overrightarrow{AB}\times\overrightarrow{AC}=(2,-4,5)}
$$

Parallelogram area:

$$
\boxed{P=3\sqrt{5}}
$$

Triangle area:

$$
\boxed{T=\frac{3\sqrt{5}}{2}\approx3.354}
$$

**Conclusion:**

The length of the cross product gives the area of the parallelogram formed by two vectors. Since a diagonal divides a parallelogram into two equal triangles, the area of triangle ABC is half of the parallelogram area. This is why the factor $\frac{1}{2}$ is necessary.
