S = [[2, 0], [0, 1]]

R = [[0, -1], [1, 0]]

x = [[1], [2]]

Calculate RSx:
First calculate Sx:

Sx = [[2, 0], [0, 1]] × [[1], [2]]

Sx = [[2], [2]]

Now calculate R(Sx):

RSx = [[0, -1], [1, 0]] × [[2], [2]]

RSx = [[-2], [2]]

Calculate SRx:
First calculate Rx:

Rx = [[0, -1], [1, 0]] × [[1], [2]]

Rx = [[-2], [1]]

Now calculate S(Rx):

SRx = [[2, 0], [0, 1]] × [[-2], [1]]

SRx = [[-4], [1]]

Comparison:
RSx = [[-2], [2]]

SRx = [[-4], [1]]

The results are different because matrix multiplication is not commutative. The order of transformations matters. Scaling and rotation produce different results depending on which operation is performed first.

