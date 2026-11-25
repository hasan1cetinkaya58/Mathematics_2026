## Exercise 9: Cross Product as a Perpendicular Direction

### Question

Given the vectors:

$$
u=(1,2,0), \qquad v=(0,1,3)
$$

1. Compute \(u\times v\).
2. Use dot products to check perpendicularity to both vectors.
3. Compute \(v\times u\).
4. Compare the results.

---

### Solution

**1. Computing the Cross Product \(u\times v\)**

The cross product of two vectors in three-dimensional space produces a new vector that is perpendicular to both original vectors.

The cross product formula is:

$$
u\times v=
(u_2v_3-u_3v_2,\;
u_3v_1-u_1v_3,\;
u_1v_2-u_2v_1)
$$

Given:

$$
u=(1,2,0), \qquad v=(0,1,3)
$$

Substituting the components:

$$
u\times v=
(2\cdot3-0\cdot1,\;
0\cdot0-1\cdot3,\;
1\cdot1-2\cdot0)
$$

Calculating each component:

$$
u\times v=(6,-3,1)
$$

Therefore:

$$
\boxed{u\times v=(6,-3,1)}
$$

**2. Checking Perpendicularity Using Dot Products**

To verify that the cross product is perpendicular to both original vectors, we calculate two dot products.

A vector is perpendicular to another vector if their dot product is zero.

First, check perpendicularity to \(u\).

We have:

$$
u=(1,2,0)
$$

$$
u\times v=(6,-3,1)
$$

Calculate the dot product:

$$
(u\times v)\cdot u
$$

$$
=6\cdot1+(-3)\cdot2+1\cdot0
$$

$$
=6-6+0
$$

$$
=0
$$

Therefore:

$$
\boxed{(u\times v)\cdot u=0}
$$

The cross product is perpendicular to \(u\).

Now, check perpendicularity to \(v\).

We have:

$$
v=(0,1,3)
$$

Calculate the dot product:

$$
(u\times v)\cdot v
$$

$$
=6\cdot0+(-3)\cdot1+1\cdot3
$$

$$
=0-3+3
$$

$$
=0
$$

Therefore:

$$
\boxed{(u\times v)\cdot v=0}
$$

The cross product is also perpendicular to \(v\).

Both checks confirm the perpendicularity of the result.

**3. Computing the Cross Product \(v\times u\)**

Now we reverse the order of the original vectors.

Using the cross product formula:

$$
v\times u=
(v_2u_3-v_3u_2,\;
v_3u_1-v_1u_3,\;
v_1u_2-v_2u_1)
$$

Substituting the components:

$$
v\times u=
(1\cdot0-3\cdot2,\;
3\cdot1-0\cdot0,\;
0\cdot2-1\cdot1)
$$

Calculating each component:

$$
v\times u=(-6,3,-1)
$$

Therefore:

$$
\boxed{v\times u=(-6,3,-1)}
$$

**4. Comparing the Results**

From our calculations:

$$
u\times v=(6,-3,1)
$$

$$
v\times u=(-6,3,-1)
$$

Comparing the two results, we can see that every component has the opposite sign.

Therefore:

$$
\boxed{v\times u=-(u\times v)}
$$

This demonstrates that the cross product is anti-commutative.

Changing the order of the vectors reverses the direction of the resulting vector, but its length remains unchanged.

Geometrically, both results are perpendicular to the same two original vectors, but they point in opposite directions.

---

### Final Results

Cross product:

$$
\boxed{u\times v=(6,-3,1)}
$$

Perpendicularity checks:

$$
\boxed{(u\times v)\cdot u=0}
$$

$$
\boxed{(u\times v)\cdot v=0}
$$

Reversed cross product:

$$
\boxed{v\times u=(-6,3,-1)}
$$

Comparison:

$$
\boxed{v\times u=-(u\times v)}
$$

**Conclusion:** The cross product produces a vector perpendicular to both original vectors. Reversing the order of the vectors changes the direction of the result but preserves its magnitude. This shows that the cross product is anti-commutative.
