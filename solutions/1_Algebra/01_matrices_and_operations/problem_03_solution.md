
# Exercise 3: When Can Matrices Be Multiplied?

## Question

The matrix sizes are:

$$
A \in \mathbb{R}^{2 \times 3}, \quad
B \in \mathbb{R}^{3 \times 4}, \quad
C \in \mathbb{R}^{4 \times 2}, \quad
D \in \mathbb{R}^{2 \times 2}.
$$

For the products

$$
AB,\quad BA,\quad BC,\quad CB,\quad AC,\quad CA,\quad AD,\quad DA
$$

determine whether they are defined. If so, state the size of the result. Justify each decision using the dimension compatibility condition.

## Solution

### 1. Matrix Multiplication Rule

Matrix multiplication is defined only when the number of columns of the first matrix equals the number of rows of the second matrix.

In general, if

$$
X \in \mathbb{R}^{m \times n}
\quad \text{and} \quad
Y \in \mathbb{R}^{p \times q},
$$

then the product $XY$ is defined if and only if

$$
n=p.
$$

When the product is defined, its resulting size is

$$
m \times q.
$$

We apply this rule to each product below.

### 2. Checking Each Product

#### 1. Product AB

The dimensions are:

$$
A: 2 \times 3,\qquad B: 3 \times 4.
$$

The number of columns of $A$ is 3, and the number of rows of $B$ is 3.

Since these numbers are equal, the product is defined.

The resulting size is determined by the outer dimensions:

$$
AB: (2 \times \cancel{3})(\cancel{3} \times 4)
$$

$$
\boxed{AB \text{ is defined and has size } 2 \times 4.}
$$

#### 2. Product BA

The dimensions are:

$$
B: 3 \times 4,\qquad A: 2 \times 3.
$$

The number of columns of $B$ is 4, while the number of rows of $A$ is 2.

Since $4 \neq 2$, the product is not defined.

$$
\boxed{BA \text{ is not defined.}}
$$

#### 3. Product BC

The dimensions are:

$$
B: 3 \times 4,\qquad C: 4 \times 2.
$$

The number of columns of $B$ is 4, and the number of rows of $C$ is 4.

Since these numbers are equal, the product is defined.

The resulting size is:

$$
BC: (3 \times \cancel{4})(\cancel{4} \times 2)
$$

$$
\boxed{BC \text{ is defined and has size } 3 \times 2.}
$$

#### 4. Product CB

The dimensions are:

$$
C: 4 \times 2,\qquad B: 3 \times 4.
$$

The number of columns of $C$ is 2, while the number of rows of $B$ is 3.

Since $2 \neq 3$, the product is not defined.

$$
\boxed{CB \text{ is not defined.}}
$$

#### 5. Product AC

The dimensions are:

$$
A: 2 \times 3,\qquad C: 4 \times 2.
$$

The number of columns of $A$ is 3, while the number of rows of $C$ is 4.

Since $3 \neq 4$, the product is not defined.

$$
\boxed{AC \text{ is not defined.}}
$$

#### 6. Product CA

The dimensions are:

$$
C: 4 \times 2,\qquad A: 2 \times 3.
$$

The number of columns of $C$ is 2, and the number of rows of $A$ is 2.

Since these numbers are equal, the product is defined.

The resulting size is:

$$
CA: (4 \times \cancel{2})(\cancel{2} \times 3)
$$

$$
\boxed{CA \text{ is defined and has size } 4 \times 3.}
$$

#### 7. Product AD

The dimensions are:

$$
A: 2 \times 3,\qquad D: 2 \times 2.
$$

The number of columns of $A$ is 3, while the number of rows of $D$ is 2.

Since $3 \neq 2$, the product is not defined.

$$
\boxed{AD \text{ is not defined.}}
$$

#### 8. Product DA

The dimensions are:

$$
D: 2 \times 2,\qquad A: 2 \times 3.
$$

The number of columns of $D$ is 2, and the number of rows of $A$ is 2.

Since these numbers are equal, the product is defined.

The resulting size is:

$$
DA: (2 \times \cancel{2})(\cancel{2} \times 3)
$$

$$
\boxed{DA \text{ is defined and has size } 2 \times 3.}
$$

### 3. Summary of Results

| Product | Compatibility condition | Result |
|---|---|---|
| $AB$ | $3 = 3$ | Defined, $2 \times 4$ |
| $BA$ | $4 \neq 2$ | Not defined |
| $BC$ | $4 = 4$ | Defined, $3 \times 2$ |
| $CB$ | $2 \neq 3$ | Not defined |
| $AC$ | $3 \neq 4$ | Not defined |
| $CA$ | $2 = 2$ | Defined, $4 \times 3$ |
| $AD$ | $3 \neq 2$ | Not defined |
| $DA$ | $2 = 2$ | Defined, $2 \times 3$ |

### 4. Final Conclusion

The products $AB$, $BC$, $CA$, and $DA$ are defined because the number of columns of the first matrix equals the number of rows of the second matrix.

The products $BA$, $CB$, $AC$, and $AD$ are not defined because their inner dimensions do not match.

Therefore, out of the eight products, four are defined and four are not defined.

This confirms that matrix multiplication depends on dimension compatibility, not simply on whether two matrices are given.
