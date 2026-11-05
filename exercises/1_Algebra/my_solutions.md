# Mathematics 2026 – Solutions
## 1. Algebra – Matrices and Basic Operations

### Exercise 1. Matrix Size and Entries

Given:

A = [[2, -1, 3], [0, 4, 5]]

B = [[1, 0], [-2, 3], [4, 1]]

1. The size of matrix A is 2 × 3.
2. The size of matrix B is 3 × 2.

The requested entries are:

- a12 = -1
- a23 = 3
- b21 = -2
- b32 = 1

The second row of A is:

[0, 4, 5]

The first column of B is:

[1, -2, 4]ᵀ

Explanation:
A matrix size is determined by its number of rows and columns. The first index represents the row, and the second index represents the column.

### Exercise 2. Addition and Scalar Multiplication

Given:

A = [[1, 2], [-1, 3]]

B = [[4, -2], [0, 5]]

**1. Addition**

A + B = [[1+4, 2-2], [-1+0, 3+5]]

A + B = [[5, 0], [-1, 8]]

**2. Subtraction**

A - B = [[1-4, 2-(-2)], [-1-0, 3-5]]

A - B = [[-3, 4], [-1, -2]]

**3. Scalar multiplication**

3A = [[3, 6], [-3, 9]]

2B = [[8, -4], [0, 10]]

3A - 2B = [[3-8, 6-(-4)], [-3-0, 9-10]]

3A - 2B = [[-5, 10], [-3, -1]]

Explanation:
Matrix addition and subtraction are possible only when both matrices have the same dimensions because corresponding entries must be combined.

### Exercise 3. When Can Matrices Be Multiplied?

The matrix sizes are:

A: 2 × 3
B: 3 × 4
C: 4 × 2
D: 2 × 2

A product XY is defined when the number of columns of X equals the number of rows of Y.

- AB: Defined, result size 2 × 4.
- BA: Not defined (4 ≠ 2).
- BC: Defined, result size 3 × 2.
- CB: Not defined (2 ≠ 3).
- AC: Not defined (3 ≠ 4).
- CA: Defined, result size 4 × 3.
- AD: Not defined (3 ≠ 2).
- DA: Defined, result size 2 × 3.

Explanation:
Matrix multiplication requires compatible dimensions. The inner dimensions must be equal, and the result has the outer dimensions.
Matrix multiplication is possible when the inner dimensions are equal. The result has the outer dimensions
### Exercise 4. Matrix Multiplication and Noncommutativity

Given:

A = [[1, 2], [0, 1]]

B = [[2, 0], [3, 1]]

**1. Calculate AB**

AB = [[1×2+2×3, 1×0+2×1],
      [0×2+1×3, 0×0+1×1]]

AB = [[8, 2], [3, 1]]

**2. Calculate BA**

BA = [[2×1+0×0, 2×2+0×1],
      [3×1+1×0, 3×2+1×1]]

BA = [[2, 4], [3, 7]]

Therefore:

AB ≠ BA

Explanation:
Matrix multiplication is not generally commutative. Changing the order of the matrices can produce a different result.

### Exercise 5. Matrix Times Vector

Given:

A = [[2, -1], [1, 3]]

x = [4, 2]ᵀ

Calculate Ax:

Ax = [[2×4 + (-1)×2],
      [1×4 + 3×2]]

Ax = [6, 10]ᵀ

The columns of A are:

c1 = [2, 1]ᵀ

c2 = [-1, 3]ᵀ

Expressing Ax as a linear combination:

Ax = 4c1 + 2c2

Ax = 4[2, 1]ᵀ + 2[-1, 3]ᵀ

Ax = [8, 4]ᵀ + [-2, 6]ᵀ

Ax = [6, 10]ᵀ

Explanation:
Multiplying a matrix by a vector is equivalent to taking a linear combination of the columns of the matrix, using the vector entries as coefficients.

### Exercise 6. Transpose

Given:

A = [[1, 2, 3], [4, 5, 6]]

B = [[1, 0], [2, 1], [-1, 3]]

**1. Calculate Aᵀ**

Aᵀ = [[1, 4], [2, 5], [3, 6]]

**2. Calculate Bᵀ**

Bᵀ = [[1, 2, -1], [0, 1, 3]]

**3. Calculate AB**

AB = [[1×1+2×2+3×(-1), 1×0+2×1+3×3],
      [4×1+5×2+6×(-1), 4×0+5×1+6×3]]

AB = [[2, 11], [8, 23]]

**4. Verify the transpose property**

(AB)ᵀ = [[2, 8], [11, 23]]

BᵀAᵀ = [[2, 8], [11, 23]]

Therefore:

(AB)ᵀ = BᵀAᵀ

Explanation:
The transpose of a product reverses the order of the factors. This is an important property of matrix multiplication.
## Exercise 7. Identity Matrix, Zero Matrix, and Powers

Given:

A = [[2, 1], [0, 2]]

1. Calculate AI:

AI = [[2, 1], [0, 2]]

2. Calculate IA:

IA = [[2, 1], [0, 2]]

3. Calculate A + 0:

A + 0 = [[2, 1], [0, 2]]

4. Calculate A²:

A² = [[2×2+1×0, 2×1+1×2],
      [0×2+2×0, 0×1+2×2]]

A² = [[4, 4], [0, 4]]

5. Calculate A³:

A³ = A² × A

A³ = [[4, 4], [0, 4]] × [[2, 1], [0, 2]]

A³ = [[8, 12], [0, 8]]

Explanation:

The identity matrix I does not change a matrix when multiplied by it. The zero matrix 0 does not change a matrix when added to it. Successive powers of A show a regular pattern.

---

## Exercise 8. Row Operations and Their Reversibility

Given:

A = [[1, 2, -1],
     [2, 4, 1],
     [-1, 1, 3]]

Step 1: R2 ← R2 - 2R1

R2 = [2, 4, 1] - 2[1, 2, -1]

R2 = [0, 0, 3]

Matrix after Step 1:

[[1, 2, -1],
 [0, 0, 3],
 [-1, 1, 3]]

Reverse operation:

R2 ← R2 + 2R1

Step 2: R3 ← R3 + R1

R3 = [-1, 1, 3] + [1, 2, -1]

R3 = [0, 3, 2]

Matrix after Step 2:

[[1, 2, -1],
 [0, 0, 3],
 [0, 3, 2]]

Reverse operation:

R3 ← R3 - R1

Step 3: Interchange R2 and R3

Matrix after Step 3:

[[1, 2, -1],
 [0, 3, 2],
 [0, 0, 3]]

Reverse operation:

Interchange R2 and R3 again.

Explanation:

All three row operations are reversible. Each operation has an inverse that restores the original matrix.

---

## Exercise 9. Composing Transformations

Given:

S = [[2, 0], [0, 1]]

R = [[0, -1], [1, 0]]

x = [[1], [2]]

1. Calculate RSx:

First calculate Sx:

Sx = [[2, 0], [0, 1]] × [[1], [2]]

Sx = [[2], [2]]

Now calculate R(Sx):

RSx = [[0, -1], [1, 0]] × [[2], [2]]

RSx = [[-2], [2]]

2. Calculate SRx:

First calculate Rx:

Rx = [[0, -1], [1, 0]] × [[1], [2]]

Rx = [[-2], [1]]

Now calculate S(Rx):

SRx = [[2, 0], [0, 1]] × [[-2], [1]]

SRx = [[-4], [1]]

3. Comparison:

RSx = [[-2], [2]]

SRx = [[-4], [1]]

The results are different because matrix multiplication is not commutative. The order of transformations matters. Scaling and rotation produce different results depending on which operation is performed first.

---

## Exercise 10. Columns of a Matrix Product

Given:

A = [[1, 2, 0],
     [0, 1, 1]]

B = [[1, 2],
     [-1, 0],
     [3, 1]]

The columns of B are:

b1 = [[1], [-1], [3]]

b2 = [[2], [0], [1]]

1. Compute Ab1 and Ab2:

Ab1 = [[1, 2, 0], [0, 1, 1]] × [[1], [-1], [3]]

Ab1 = [[1 - 2 + 0], [-1 + 3]]

Ab1 = [[-1], [2]]

Ab2 = [[1, 2, 0], [0, 1, 1]] × [[2], [0], [1]]

Ab2 = [[2 + 0 + 0], [0 + 1]]

Ab2 = [[2], [1]]

2. Compute AB:

AB = [[-1, 2],
      [2, 1]]

3. Comparison:

The columns of AB are exactly the vectors Ab1 and Ab2. This shows that matrix multiplication can be understood as applying matrix A to each column of matrix B.

---

## Exercise 11. When Do Matrices Commute?

Given:

A = [[1, 1],
     [0, 1]]

B = [[a, b],
     [c, d]]

We need to find the conditions under which AB = BA.

First calculate AB:

AB = [[1, 1], [0, 1]] × [[a, b], [c, d]]

AB = [[a + c, b + d],
      [c, d]]

Now calculate BA:

BA = [[a, b], [c, d]] × [[1, 1], [0, 1]]

BA = [[a, a + b],
      [c, c + d]]

Since AB = BA, compare corresponding entries:

a + c = a
b + d = a + b
c = c
d = c + d

Therefore:

c = 0

d = a

Final answer:

B = [[a, b],
     [0, a]]

where a and b can be any real numbers.

Explanation:

Matrix multiplication is not generally commutative. However, for this particular matrix A, the matrices commute when c = 0 and d = a.

---

## Exercise 12. Formula for a Matrix Power

Given:

A = [[1, 1],
     [0, 1]]

1. Calculate A²:

A² = A × A

A² = [[1, 2],
      [0, 1]]

2. Calculate A³:

A³ = A² × A

A³ = [[1, 3],
      [0, 1]]

3. Calculate A⁴:

A⁴ = A³ × A

A⁴ = [[1, 4],
      [0, 1]]

4. Calculate A⁵:

A⁵ = A⁴ × A

A⁵ = [[1, 5],
      [0, 1]]

5. General formula:

Aⁿ = [[1, n],
      [0, 1]]

6. Verification:

Assume:

Aⁿ = [[1, n],
      [0, 1]]

Then:

Aⁿ⁺¹ = Aⁿ × A

Aⁿ⁺¹ = [[1, n], [0, 1]] × [[1, 1], [0, 1]]

Aⁿ⁺¹ = [[1, n + 1],
        [0, 1]]

Therefore, the formula is true for the next power as well.

Explanation:

Each multiplication increases the upper-right entry by one. This creates a simple pattern that can be generalized for any positive integer n.

---

## Exercise 13. A Recurrence Written in Matrix Form

Given:

F = [[1, 1],
     [1, 0]]

1. Calculate F²:

F² = [[2, 1],
      [1, 1]]

2. Calculate F³:

F³ = [[3, 2],
      [2, 1]]

3. Calculate F⁴:

F⁴ = [[5, 3],
      [3, 2]]

4. Calculate F⁵:

F⁵ = [[8, 5],
      [5, 3]]

5. Compare the results:

The Fibonacci sequence is:

0, 1, 1, 2, 3, 5, 8, ...

The entries of the matrix powers follow the Fibonacci sequence.

The general formula is:

Fⁿ = [[F(n+1), F(n)],
      [F(n), F(n-1)]]

where F(0) = 0 and F(1) = 1.

Explanation:

Multiplying by matrix F creates the sum of two consecutive Fibonacci numbers. This demonstrates how matrix multiplication can represent a numerical recurrence.

---

## Exercise 14. Rotation Matrices

Given:

R(θ) = [[cos θ, -sin θ],
        [sin θ, cos θ]]

We need to prove:

R(α)R(β) = R(α + β)

First calculate:

R(α)R(β) =

[[cos α, -sin α],
 [sin α, cos α]]

×

[[cos β, -sin β],
 [sin β, cos β]]

Multiplying the matrices:

= [[cos α cos β - sin α sin β,
    -cos α sin β - sin α cos β],

   [sin α cos β + cos α sin β,
    -sin α sin β + cos α cos β]]

Using the trigonometric identities:

cos(α + β) = cos α cos β - sin α sin β

sin(α + β) = sin α cos β + cos α sin β

We obtain:

R(α)R(β) =

[[cos(α + β), -sin(α + β)],
 [sin(α + β), cos(α + β)]]

Therefore:

R(α)R(β) = R(α + β)

Geometric explanation:

Applying two rotations successively is equivalent to performing one rotation by the sum of their angles. The final position depends on the total rotation angle.

---

## Exercise 15. Associativity of Multiplication and Different Calculation Paths

Given:

A = [[1, 2, 0],
     [0, 1, 1]]

B = [[1, 0],
     [2, 1],
     [-1, 3]]

C = [[2, 1],
     [0, -1]]

1. Compute (AB)C:

First calculate AB:

AB = [[1, 2, 0],
      [0, 1, 1]]

     ×

     [[1, 0],
      [2, 1],
      [-1, 3]]

AB = [[5, 2],
      [1, 4]]

Now calculate (AB)C:

(AB)C = [[5, 2],
         [1, 4]]

        ×

        [[2, 1],
         [0, -1]]

(AB)C = [[10, 3],
         [2, -3]]

2. Compute A(BC):

First calculate BC:

BC = [[1, 0],
      [2, 1],
      [-1, 3]]

     ×

     [[2, 1],
      [0, -1]]

BC = [[2, 1],
      [4, 1],
      [-2, -4]]

Now calculate A(BC):

A(BC) = [[1, 2, 0],
         [0, 1, 1]]

        ×

        [[2, 1],
         [4, 1],
         [-2, -4]]

A(BC) = [[10, 3],
         [2, -3]]

3. Compare the results:

(AB)C = [[10, 3],
         [2, -3]]

A(BC) = [[10, 3],
         [2, -3]]

Therefore:

(AB)C = A(BC)

Explanation:

Matrix multiplication is associative. Changing the grouping of the matrices does not change the final result.

However, the number of calculations can differ depending on the order of multiplication. In this example, calculating (AB)C requires fewer scalar multiplications than calculating A(BC).

This demonstrates why choosing an efficient calculation path is important.
