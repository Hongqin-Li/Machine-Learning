# Lagrange multipliers
>min f(x)
>
>s.t. g_i(x) <= 0; i = 1, ..., n
>
>h_j(x) = 0; j = 1, ..., m

  Instead of solving directly, we use the following function: 
  L(a, b, x)= f(x) + a*g(x)+b*h(x)

1. L(a, b, x)对x求导为零；

2. h(x) =0;

3. a*g(x) = 0;
