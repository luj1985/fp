##  Lambda Calculus

Lambda expressions are composed of

- variables v1, v2, ..., vn, ...
- the abstraction symbols lambda 'λ' and dot '.'
- parentheses ( )

The set of lambda expressions, Λ, can be defined inductively:

- If x is a variable, then x ∈ Λ
- If x is a variable and M ∈ Λ, then (λx.M) ∈ Λ
- If M, N ∈ Λ, then (M N) ∈ Λ
