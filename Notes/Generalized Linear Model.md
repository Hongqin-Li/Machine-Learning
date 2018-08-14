# Generalized Linear Model
## Exponential Family
P( y | η ) = b( y ) · e<sup><sup/>(η<sup>T</sup> · T( y ) - a( η ) )

In most case, we can't directly know what η is.
(e.g. Gaussian's μ( mean ), Bernoulli's Φ.)
But we can work it out as a function of μ or Φ or something else.
## Three assumptions
1. P( y | x ; Θ ) ∼ ExponentialFamily( η )

the ";" here means : given x and Θ, in other words, x and Θ are invariant.

2. h<sub>Θ</sub>(x) = E[ y | η ]

Here is an improtant property of the exponential family:

  E[ y | η ] = d / dη ( a( η ) ) **( depends only on η, not y! )**
  
  so by intuition( or by the assumption ), h<sub>Θ</sub>(x) = E[ y | η ], then we can easily calculate hypothesis function through the model.
  

3. η = θ<sup>T</sup>x
( Or η<sub>i</sub> = θ<sub>i</sub><sup>T</sup>x )

Just for convenience. Also, we can have some nonlinear forms, but that works more difficultly.
