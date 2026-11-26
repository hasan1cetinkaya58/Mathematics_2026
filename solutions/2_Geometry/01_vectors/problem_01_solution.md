
# Exercise 1: Vector Operations and Their Meaning

## Question

Given the vectors:

$$
u = (2,-1,3), \qquad v = (-1,4,2)
$$

Compute:

1. `u + v`
2. `u - v`
3. `3u - 2v`

Then verify that:

$$
(u+v)-v=u
$$

Finally, explain geometrically what adding two vectors means.

## Solution

### 1. Vector Addition

To add two vectors, we add their corresponding components.

$$
u+v=(2,-1,3)+(-1,4,2)
$$

$$
=(2-1,-1+4,3+2)
$$

$$
\boxed{u+v=(1,3,5)}
$$

### 2. Vector Subtraction

To subtract two vectors, we subtract their corresponding components.

$$
u-v=(2,-1,3)-(-1,4,2)
$$

$$
=(2+1,-1-4,3-2)
$$

$$
\boxed{u-v=(3,-5,1)}
$$

### 3. Scalar Multiplication and Subtraction

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
=(6+2,-3-8,9-4)
$$

$$
\boxed{3u-2v=(8,-11,5)}
$$

### 4. Verification of the Identity

We need to verify:

`(u+v)-v=u`

From the first calculation:

$$
u+v=(1,3,5)
$$

Substitute this result:

$$
(u+v)-v=(1,3,5)-(-1,4,2)
$$

$$
=(1+1,3-4,5-2)
$$

$$
=(2,-1,3)
$$

Since:

$$
u=(2,-1,3)
$$

we obtain:

$$
\boxed{(u+v)-v=u}
$$

Therefore, the identity is verified.

### 5. Geometric Interpretation

Geometrically, adding two vectors means combining their directions and magnitudes to obtain a resultant vector.

This can be explained using the **head-to-tail method**:

1. First, draw vector `u`.
2. Place the starting point of vector `v` at the endpoint of `u`.
3. Draw a new vector from the starting point of `u` to the endpoint of `v`.

The resulting vector represents `u+v`.

This is also known as the triangle rule of vector addition.

Vector addition can also be represented using the parallelogram rule. When two vectors start at the same point, their sum is represented by the diagonal of the parallelogram formed by those vectors.

In this exercise, the vectors belong to `R^3`, so their geometric representation is in three-dimensional space.

## Final Results

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

**Conclusion:** Vector operations are performed component by component. Geometrically, vector addition combines two displacements into one resultant displacement.
