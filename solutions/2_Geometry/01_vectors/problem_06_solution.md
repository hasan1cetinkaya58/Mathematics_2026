## Exercise 6: Projection and Perpendicular Component

### Question

Given the vectors:

$$
u=(4,2), \qquad v=(1,1)
$$

1. Find the projection of \(u\) onto the direction of \(v\).
2. Compute the perpendicular component:

$$
r=u-p
$$

where \(p\) is the projection of \(u\) onto \(v\).

3. Verify that \(r\cdot v=0\).
4. Explain this result geometrically.

---

### Solution

**1. Finding the Projection of \(u\) onto \(v\)**

The projection of vector \(u\) onto vector \(v\) represents the component of \(u\) that lies in the direction of \(v\).

We denote the projection by \(p\).

The projection formula is:

$$
p=\frac{u\cdot v}{v\cdot v}v
$$

First, calculate the dot product of \(u\) and \(v\):

$$
u\cdot v=(4)(1)+(2)(1)
$$

$$
=4+2=6
$$

Next, calculate the dot product of \(v\) with itself:

$$
v\cdot v=(1)(1)+(1)(1)
$$

$$
=1+1=2
$$

Now substitute these values into the projection formula:

$$
p=\frac{6}{2}(1,1)
$$

$$
=3(1,1)
$$

Therefore:

$$
\boxed{p=(3,3)}
$$

**2. Computing the Perpendicular Component**

The perpendicular component is obtained by subtracting the projection from the original vector.

The formula is:

$$
r=u-p
$$

Substituting the calculated values:

$$
r=(4,2)-(3,3)
$$

Subtracting the corresponding components:

$$
r=(4-3,\,2-3)
$$

Therefore:

$$
\boxed{r=(1,-1)}
$$

**3. Verifying That the Perpendicular Component Is Orthogonal to \(v\)**

To verify that \(r\) is perpendicular to \(v\), we calculate their dot product.

We have:

$$
r=(1,-1), \qquad v=(1,1)
$$

Using the dot product formula:

$$
r\cdot v=(1)(1)+(-1)(1)
$$

$$
=1-1
$$

$$
=0
$$

Therefore:

$$
\boxed{r\cdot v=0}
$$

Since the dot product is zero, the vectors are perpendicular.

The result is verified.

**4. Geometric Interpretation**

The original vector \(u\) can be decomposed into two components:

- The projection \(p=(3,3)\), which is parallel to \(v\).
- The perpendicular component \(r=(1,-1)\), which is orthogonal to \(v\).

This means that the original vector is the sum of its parallel and perpendicular components.

Mathematically:

$$
u=p+r
$$

Substituting the values:

$$
(4,2)=(3,3)+(1,-1)
$$

This decomposition shows that the projection represents the part of \(u\) in the direction of \(v\), while \(r\) represents the remaining perpendicular part.

Geometrically, the projection is the closest point on the line through the origin in the direction of \(v\) to the endpoint of \(u\).

---

### Final Results

Projection:

$$
\boxed{p=(3,3)}
$$

Perpendicular component:

$$
\boxed{r=(1,-1)}
$$

Verification:

$$
\boxed{r\cdot v=0}
$$

Vector decomposition:

$$
\boxed{u=(3,3)+(1,-1)}
$$

**Conclusion:** A vector can be decomposed into parallel and perpendicular components relative to another vector. The projection gives the parallel component, while subtracting it from the original vector gives the perpendicular component. Their dot product is zero, confirming their orthogonality.
