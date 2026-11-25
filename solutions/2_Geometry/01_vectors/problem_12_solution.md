
# Exercise 12: A Normal Vector to a Plane

## Question

Given the points:

$$
A=(1,0,2), \quad B=(2,1,0), \quad C=(0,3,1).
$$

1. Construct two vectors lying in the plane.
2. Find a vector perpendicular to both vectors using the cross product.
3. Check the perpendicularity using dot products.

---

## Solution

### 1. Constructing Two Vectors in the Plane

To construct vectors lying in the plane, we subtract the coordinates of the starting point from the coordinates of the ending point.

First, construct the vector from A to B:

$$
\overrightarrow{AB}=B-A
$$

Substituting the coordinates:

$$
\overrightarrow{AB}
=(2,1,0)-(1,0,2)
$$

Therefore:

$$
\overrightarrow{AB}=(1,1,-2)
$$

Now construct the vector from A to C:

$$
\overrightarrow{AC}=C-A
$$

Substituting the coordinates:

$$
\overrightarrow{AC}
=(0,3,1)-(1,0,2)
$$

Therefore:

$$
\overrightarrow{AC}=(-1,3,-1)
$$

Both vectors lie in the plane ABC because they connect points belonging to that plane.

### 2. Finding a Normal Vector Using the Cross Product

A normal vector is perpendicular to both independent direction vectors lying in the plane.

We calculate the cross product:

$$
\vec{n}=\overrightarrow{AB}\times\overrightarrow{AC}
$$

Using the cross product formula:

$$
\vec{n}=
\begin{pmatrix}
1\\
1\\
-2
\end{pmatrix}
\times
\begin{pmatrix}
-1\\
3\\
-1
\end{pmatrix}
$$

Calculating each component:

$$
\vec{n}=
\begin{pmatrix}
1(-1)-(-2)(3)\\
(-2)(-1)-1(-1)\\
1(3)-1(-1)
\end{pmatrix}
$$

Simplifying:

$$
\vec{n}=
\begin{pmatrix}
-1+6\\
2+1\\
3+1
\end{pmatrix}
$$

Therefore:

$$
\boxed{\vec{n}=(5,3,4)}
$$

This is a normal vector to the plane ABC.

### 3. Checking Perpendicularity Using Dot Products

To verify that the normal vector is perpendicular to both direction vectors, we calculate two dot products.

A vector is perpendicular to another vector if their dot product equals zero.

First, check perpendicularity to AB:

$$
\vec{n}\cdot\overrightarrow{AB}
=(5,3,4)\cdot(1,1,-2)
$$

$$
=5(1)+3(1)+4(-2)
$$

$$
=5+3-8=0
$$

Therefore:

$$
\vec{n}\cdot\overrightarrow{AB}=0
$$

Now check perpendicularity to AC:

$$
\vec{n}\cdot\overrightarrow{AC}
=(5,3,4)\cdot(-1,3,-1)
$$

$$
=5(-1)+3(3)+4(-1)
$$

$$
=-5+9-4=0
$$

Therefore:

$$
\vec{n}\cdot\overrightarrow{AC}=0
$$

Both dot products are zero, so the normal vector is perpendicular to both vectors.

### 4. Geometric Explanation

The vectors AB and AC describe two different directions lying in the plane ABC.

Their cross product produces a vector perpendicular to both directions.

Since these two direction vectors span the plane, the resulting vector is perpendicular to the entire plane.

This is why the cross product is useful for finding a normal vector to a plane.

---

## Final Results

First direction vector:

$$
\overrightarrow{AB}=(1,1,-2)
$$

Second direction vector:

$$
\overrightarrow{AC}=(-1,3,-1)
$$

Normal vector:

$$
\boxed{\vec{n}=(5,3,4)}
$$

Perpendicularity checks:

$$
\vec{n}\cdot\overrightarrow{AB}=0
$$

$$
\vec{n}\cdot\overrightarrow{AC}=0
$$

Therefore, the vector (5,3,4) is a valid normal vector to the plane ABC.
