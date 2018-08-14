# Lagrange multipliers
> min f(x)
>
> subject to
>
> g<sub>i</sub>(x) <= 0; i = 1, ..., n
>
> h<sub>j</sub>(x) = 0; j = 1, ..., m

  Instead of solving directly, we use the following function: 
  > L(α, β, x) = f(x) + Σα<sub>i</sub> · g<sub>i</sub>(x) + Σβ<sub>j</sub> · h<sub>j</sub>(x)
  > 
  > **α<sub>i</sub> >= 0**
  
  This constrain acts when
  > θ<sub>p</sub>(x) = max<sub>α,β</sub>L(α, β, x) = f(x)
  
  Without it,
  > θ<sub>p</sub>(x) = max<sub>α,β</sub>L(α, β, x) = ∞
 
  the KKT conditions :
  > 1. ∂/∂x[L(α, β, x)] = 0;
  > 2. h(x) = 0;
  > 3. **α<sub>i</sub> · g<sub>i</sub>(x) = 0;**
