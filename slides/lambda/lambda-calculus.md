##  Lambda Calculus

BNF definition:
```
<expr> ::= <identifier>
<expr> ::= λ <identifier-list>. <expr>
<expr> ::= (<expr> <expr>)
```


* α-conversion: changing bound variables (alpha);
* β-reduction: applying functions to their arguments (beta);
* η-conversion: which captures a notion of extensionality (eta).