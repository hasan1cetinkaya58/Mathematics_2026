## Exercise 4: Dot Product and Perpendicularity

### Question

Given the vectors:

$$
u=(1,2,-1), \qquad v=(2,-1,3)
$$

1. Compute the dot product \(u\cdot v\) and determine whether the vectors are perpendicular.
2. Find \(a\) so that \(w=(2,-1,a)\) is perpendicular to \(u\).
3. Check the result.

---

### Solution

**1. Computing the Dot Product and Checking Perpendicularity**

The dot product of two vectors in \(\mathbb{R}^3\) is calculated by multiplying their corresponding components and adding the results.

The formula is:

$$
u\cdot v=u_1v_1+u_2v_2+u_3v_3
$$

Substituting the given vectors:

$$
u\cdot v=(1)(2)+(2)(-1)+(-1)(3)
$$

Multiplying the corresponding components:

$$
=2-2-3
$$

$$
\boxed{u\cdot v=-3}
$$

Two nonzero vectors are perpendicular if and only if their dot product is equal to zero.

Since:

$$
u\cdot v=-3\neq 0
$$

Therefore:

$$
\boxed{\text{The vectors are not perpendicular.}}
$$

**2. Finding the Value of \(a\)**

We are given:

$$
u=(1,2,-1)
$$

$$
w=(2,-1,a)
$$

To make the vectors perpendicular, their dot product must be equal to zero.

The perpendicularity condition is:

$$
u\cdot w=0
$$

Using the dot product formula:

$$
(1)(2)+(2)(-1)+(-1)(a)=0
$$

Simplifying:

$$
2-2-a=0
$$

$$
-a=0
$$

Therefore:

$$
\boxed{a=0}
$$

The required vector is:

$$
\boxed{w=(2,-1,0)}
$$

**3. Checking the Result**

To verify our answer, we calculate the dot product of \(u\) and the new vector \(w\).

We have:

$$
u=(1,2,-1)
$$

$$
w=(2,-1,0)
$$

Calculating the dot product:

$$
u\cdot w=(1)(2)+(2)(-1)+(-1)(0)
$$

$$
=2-2+0
$$

$$
=0
$$

Therefore:

$$
\boxed{u\cdot w=0}
$$

Since the dot product is zero, the vectors are perpendicular.

The result is verified.

**4. Geometric Interpretation**

The dot product provides a way to determine the angle between two nonzero vectors.

Its relationship with the angle is given by:

$$
u\cdot v=\|u\|\|v\|\cos\theta
$$

When two vectors are perpendicular, the angle between them is \(90^\circ\).

Since:

$$
\cos 90^\circ=0
$$

Their dot product must also be zero.

In the second part of this exercise, we used this property to find the unknown component \(a\) and construct a vector perpendicular to \(u\).

---

### Final Results

For the first pair of vectors:

$$
\boxed{u\cdot v=-3}
$$

$$
\boxed{\text{Not perpendicular}}
$$

For the second pair:

$$
\boxed{a=0}
$$

$$
\boxed{w=(2,-1,0)}
$$

Verification:

$$
\boxed{u\cdot w=0}
$$

**Conclusion:** The dot product is useful for testing perpendicularity and finding unknown vector components. Two nonzero vectors are perpendicular exactly when their dot product is zero.
