Rotation Matrices
Given:

R(θ) = [[cos θ, -sin θ], [sin θ, cos θ]]

We need to prove:

R(α)R(β) = R(α + β)

First calculate:

R(α)R(β) =

[[cos α, -sin α], [sin α, cos α]]

×

[[cos β, -sin β], [sin β, cos β]]

Multiplying the matrices:

= [[cos α cos β - sin α sin β, -cos α sin β - sin α cos β],

[sin α cos β + cos α sin β, -sin α sin β + cos α cos β]]

Using the trigonometric identities:

cos(α + β) = cos α cos β - sin α sin β

sin(α + β) = sin α cos β + cos α sin β

We obtain:

R(α)R(β) =

[[cos(α + β), -sin(α + β)], [sin(α + β), cos(α + β)]]

Therefore:

R(α)R(β) = R(α + β)

Geometric explanation:

Applying two rotations successively is equivalent to performing one rotation by the sum of their angles. The final position depends on the total rotation angle.
