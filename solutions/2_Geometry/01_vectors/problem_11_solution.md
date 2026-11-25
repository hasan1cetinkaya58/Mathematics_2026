## Exercise 11: Decomposition into Parallel and Perpendicular Components

### Question

Given the vectors:

$$
u=(3,4), \qquad v=(1,2)
$$

1. Decompose $u$ into components parallel and perpendicular to $v$.
2. Verify that $u=u_{\parallel}+u_{\perp}$.
3. Verify that $u_{\perp}\cdot v=0$.
4. Explain why these are two independent checks of correctness.

---

### Solution

**1. Finding the Parallel Component**

To decompose a vector into parallel and perpendicular components, we first calculate the projection of $u$ onto $v$.

The projection formula is:

$$
u_{\parallel}=
\frac{u\cdot v}{v\cdot v}v
$$

Given:

$$
u=(3,4), \qquad v=(1,2)
$$

First, calculate the dot product of the two vectors:

$$
u\cdot v=3\cdot1+4\cdot2
$$

$$
=3+8=11
$$

Now calculate the dot product of $v$ with itself:

$$
v\cdot v=1^2+2^2
$$

$$
=1+4=5
$$

Substitute these values into the projection formula:

$$
u_{\parallel}=\frac{11}{5}(1,2)
$$

Multiply each component by $\frac{11}{5}$:

$$
u_{\parallel}=
\left(\frac{11}{5},\frac{22}{5}\right)
$$

Therefore, the parallel component is:

$$
\boxed{
u_{\parallel}=
\left(\frac{11}{5},\frac{22}{5}\right)
}
$$

**2. Finding the Perpendicular Component**

The original vector is the sum of its parallel and perpendicular components.

Therefore:

$$
u=u_{\parallel}+u_{\perp}
$$

Rearranging the equation:

$$
u_{\perp}=u-u_{\parallel}
$$

Substitute the known values:

$$
u_{\perp}=
(3,4)-
\left(\frac{11}{5},\frac{22}{5}\right)
$$

Subtract the corresponding components:

$$
u_{\perp}=
\left(
3-\frac{11}{5},
4-\frac{22}{5}
\right)
$$

Convert the integers into fractions:

$$
u_{\perp}=
\left(
\frac{15}{5}-\frac{11}{5},
\frac{20}{5}-\frac{22}{5}
\right)
$$

Simplify:

$$
u_{\perp}=
\left(\frac{4}{5},-\frac{2}{5}\right)
$$

Therefore, the perpendicular component is:

$$
\boxed{
u_{\perp}=
\left(\frac{4}{5},-\frac{2}{5}\right)
}
$$

**3. First Check: Verifying the Decomposition**

We must verify that the sum of the parallel and perpendicular components reconstructs the original vector.

The required condition is:

$$
u=u_{\parallel}+u_{\perp}
$$

Substitute our calculated components:

$$
(3,4)=
\left(\frac{11}{5},\frac{22}{5}\right)
+
\left(\frac{4}{5},-\frac{2}{5}\right)
$$

Add the corresponding components:

$$
=
\left(
\frac{11}{5}+\frac{4}{5},
\frac{22}{5}-\frac{2}{5}
\right)
$$

$$
=
\left(\frac{15}{5},\frac{20}{5}\right)
$$

$$
=(3,4)
$$

Therefore:

$$
\boxed{u=u_{\parallel}+u_{\perp}}
$$

The first check is satisfied because the two components reconstruct the original vector exactly.

**4. Second Check: Verifying Perpendicularity**

The perpendicular component must be perpendicular to $v$.

Two vectors are perpendicular if their dot product is zero.

The required condition is:

$$
u_{\perp}\cdot v=0
$$

Substitute the calculated values:

$$
\left(\frac{4}{5},-\frac{2}{5}\right)
\cdot(1,2)
$$

Calculate the dot product:

$$
=\frac{4}{5}\cdot1+
\left(-\frac{2}{5}\right)\cdot2
$$

$$
=\frac{4}{5}-\frac{4}{5}
$$

$$
=0
$$

Therefore:

$$
\boxed{u_{\perp}\cdot v=0}
$$

The second check is also satisfied. This confirms that the perpendicular component is indeed perpendicular to $v$.

**5. Why Are These Two Independent Checks Important?**

The two checks verify different properties of the decomposition.

**First check: Reconstruction**

$$
u=u_{\parallel}+u_{\perp}
$$

This confirms that the two components add up to the original vector. No part of the original vector is lost or added.

**Second check: Perpendicularity**

$$
u_{\perp}\cdot v=0
$$

This confirms that the perpendicular component forms a right angle with $v$.

These checks are independent because satisfying one condition does not automatically guarantee the other.

For example, two components could add up to the original vector but still not be perpendicular to each other.

Similarly, a vector could be perpendicular to $v$ without the two components reconstructing the original vector.

Together, the two checks establish that the decomposition is correct.

Additionally, the parallel component is a scalar multiple of $v$:

$$
u_{\parallel}=\frac{11}{5}v
$$

This confirms that it has the same direction as $v$.

---

### Final Results

Parallel component:

$$
\boxed{
u_{\parallel}=
\left(\frac{11}{5},\frac{22}{5}\right)
}
$$

Perpendicular component:

$$
\boxed{
u_{\perp}=
\left(\frac{4}{5},-\frac{2}{5}\right)
}
$$

Reconstruction check:

$$
\boxed{
u_{\parallel}+u_{\perp}=(3,4)=u
}
$$

Perpendicularity check:

$$
\boxed{
u_{\perp}\cdot v=0
}
$$

**Conclusion:**

The original vector $u=(3,4)$ has been successfully decomposed into a parallel component and a perpendicular component relative to $v=(1,2)$. The reconstruction check confirms that both components reproduce the original vector, while the dot product check confirms perpendicularity. Together, these two independent checks verify the correctness of the decomposition.
