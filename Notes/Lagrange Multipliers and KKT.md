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
  > θ<sub>p</sub>(x) = max<sub>α,β:α<sub>i</sub>>=0</sub>{L(α, β, x)} = f(x) 
  
  Because g<sub>i</sub>(x) <= 0, then α<sub>i</sub> · g<sub>i</sub>(x) <= 0. So just  set α = 0 to get the maximum.
  
  Without it,
  > θ<sub>p</sub>(x) = max<sub>α,β</sub>L(α, β, x) = ∞
 
# “max min” of a function is less than or equal to the “min max”
  min<sub>y</sub>max<sub>x</sub>f(x, y) >= || min<sub>y</sub>f(x, y) ||

 
  the KKT conditions :
  > 1. ∂/∂x[L(α, β, x)] = 0;
  > 2. h(x) = 0;
  > 3. **α<sub>i</sub> · g<sub>i</sub>(x) = 0;**


![](Machine-Learning/Resources/Screenshot_2018-08-15-15-13-56.png)
