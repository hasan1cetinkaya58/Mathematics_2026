
# Exercise 13: Do Four Points Lie in One Plane?

## Question

Given the points:

$$
A=(0,0,0),\quad B=(1,2,0)
$$

$$
C=(0,1,1),\quad D=(2,5,1)
$$

1. Construct the vectors AB and AC.
2. Find the normal vector n = AB × AC.
3. Construct AD and check whether AD · n = 0.
4. Decide whether D lies in the plane determined by A, B, and C, and justify the criterion.

---

## Solution

### 1. Constructing the Vectors AB and AC

To construct a vector between two points, we subtract the coordinates of the starting point from the coordinates of the ending point.

First, calculate AB:

$$
\overrightarrow{AB}=B-A
$$

Substituting the coordinates:

$$
\overrightarrow{AB}
=(1,2,0)-(0,0,0)
$$

Therefore:

$$
\overrightarrow{AB}=(1,2,0)
$$

Now calculate AC:

$$
\overrightarrow{AC}=C-A
$$

Substituting the coordinates:

$$
\overrightarrow{AC}
=(0,1,1)-(0,0,0)
$$

Therefore:

$$
\overrightarrow{AC}=(0,1,1)
$$

These two vectors determine directions within the plane ABC.

### 2. Finding the Normal Vector

A normal vector is perpendicular to both direction vectors in the plane.

We calculate their cross product:

$$
\vec{n}=\overrightarrow{AB}\times\overrightarrow{AC}
$$

Substituting the components:

$$
\vec{n}=
\begin{pmatrix}
1\\
2\\
0
\end{pmatrix}
\times
\begin{pmatrix}
0\\
1\\
1
\end{pmatrix}
$$

Using the cross product formula:

$$
\vec{n}=
\begin{pmatrix}
2(1)-0(1)\\
0(0)-1(1)\\
1(1)-2(0)
\end{pmatrix}
$$

Simplifying:

$$
\vec{n}=
\begin{pmatrix}
2\\
-1\\
1
\end{pmatrix}
$$

Therefore:

$$
\boxed{\vec{n}=(2,-1,1)}
$$

This is a normal vector to the plane ABC.

### 3. Constructing AD and Checking the Dot Product

First, construct the vector AD:

$$
\overrightarrow{AD}=D-A
$$

Substituting the coordinates:

$$
\overrightarrow{AD}
=(2,5,1)-(0,0,0)
$$

Therefore:

$$
\overrightarrow{AD}=(2,5,1)
$$

Now calculate the dot product between AD and the normal vector n:

$$
\overrightarrow{AD}\cdot\vec{n}
=(2,5,1)\cdot(2,-1,1)
$$

Multiplying corresponding components:

$$
=2(2)+5(-1)+1(1)
$$

Simplifying:

$$
=4-5+1
$$

Therefore:

$$
\boxed{\overrightarrow{AD}\cdot\vec{n}=0}
$$

### 4. Determining Whether D Lies in the Plane ABC

A point D lies in the plane determined by A, B, and C if the vector AD is perpendicular to the normal vector n.

The criterion is:

$$
\overrightarrow{AD}\cdot\vec{n}=0
$$

From our calculation:

$$
\overrightarrow{AD}\cdot\vec{n}=0
$$

Therefore, the condition is satisfied.

Hence:

$$
\boxed{D\text{ lies in the plane }ABC.}
$$

Geometrically, the normal vector describes the direction perpendicular to the plane. If the dot product of AD with this normal vector is zero, AD has no component in the normal direction.

This means that D belongs to the same plane as A, B, and C.

---

## Final Results

First vector:

$$
\overrightarrow{AB}=(1,2,0)
$$

Second vector:

$$
\overrightarrow{AC}=(0,1,1)
$$

Normal vector:

$$
\boxed{\vec{n}=(2,-1,1)}
$$

Vector AD:

$$
\overrightarrow{AD}=(2,5,1)
$$

Dot product:

$$
\overrightarrow{AD}\cdot\vec{n}=0
$$

Final conclusion:

$$
\boxed{D\text{ lies in plane }ABC.}
$$
