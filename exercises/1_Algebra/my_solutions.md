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
