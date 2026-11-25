## Question

For $u=(2,-1,3)$ and $v=(-1,4,2)$, compute $u+v$, $u-v$, and $3u-2v$; verify $(u+v)-v=u$ and explain vector addition geometrically.

## Solution

Vector operations are performed coordinate by coordinate:

$$u+v=(1,3,5),\qquad u-v=(3,-5,1),$$

$$3u-2v=(6,-3,9)-(-2,8,4)=(8,-11,5).$$

The requested check gives

$$(u+v)-v=(1,3,5)-(-1,4,2)=(2,-1,3)=u.$$

Geometrically, adding vectors means placing the tail of the second vector at the head of the first; the sum is the displacement from the original tail to the final head (equivalently, the diagonal of the parallelogram).


## Exercise 1: Vector Operations and Their Meaning

### Question

Given the vectors:

$$
u = (2,-1,3), \qquad v = (-1,4,2)
$$

Compute:

1. \(u+v\)
2. \(u-v\)
3. \(3u-2v\)

Then verify that:

$$
(u+v)-v=u
$$

Finally, explain geometrically what adding two vectors means.

---

### Solution

**1. Vector Addition: \(u+v\)**

To add two vectors, we add their corresponding components.

$$
u+v=(2,-1,3)+(-1,4,2)
$$

$$
=(2-1,\,-1+4,\,3+2)
$$

$$
\boxed{u+v=(1,3,5)}
$$

**2. Vector Subtraction: \(u-v\)**

To subtract two vectors, we subtract their corresponding components.

$$
u-v=(2,-1,3)-(-1,4,2)
$$

$$
=(2+1,\,-1-4,\,3-2)
$$

$$
\boxed{u-v=(3,-5,1)}
$$

**3. Scalar Multiplication and Subtraction: \(3u-2v\)**

First, multiply each vector by its scalar.

$$
3u=3(2,-1,3)=(6,-3,9)
$$

$$
2v=2(-1,4,2)=(-2,8,4)
$$

Now subtract the resulting vectors.

$$
3u-2v=(6,-3,9)-(-2,8,4)
$$

$$
=(6+2,\,-3-8,\,9-4)
$$

$$
\boxed{3u-2v=(8,-11,5)}
$$

**4. Verification: \((u+v)-v=u\)**

We substitute the original vectors and calculate.

From the first calculation:

$$
u+v=(1,3,5)
$$

Therefore:

$$
(u+v)-v=(1,3,5)-(-1,4,2)
$$

$$
=(1+1,\,3-4,\,5-2)
$$

$$
=(2,-1,3)
$$

Since:

$$
u=(2,-1,3)
$$

We obtain:

$$
\boxed{(u+v)-v=u}
$$

The identity is verified.

**5. Geometric Interpretation**

Geometrically, adding two vectors means combining their directions and magnitudes.

The result can be understood using the **head-to-tail method**:

- First, draw vector \(u\).
- Then, place the starting point of vector \(v\) at the endpoint of \(u\).
- The resultant vector \(u+v\) starts at the beginning of \(u\) and ends at the endpoint of \(v\).

This is also known as the triangle rule of vector addition.

Vector addition can also be represented using the parallelogram rule.

In this exercise, the vectors are in \(\mathbb{R}^3\), so their geometric representation is in three-dimensional space.

---

### Final Results

$$
\boxed{u+v=(1,3,5)}
$$

$$
\boxed{u-v=(3,-5,1)}
$$

$$
\boxed{3u-2v=(8,-11,5)}
$$

$$
\boxed{(u+v)-v=u}
$$

**Conclusion:** Vector operations are performed component by component. Geometrically, vector addition combines two displacements into one resultant displacement, while subtraction reverses the direction of the vector being subtracted.
