### Lambda calculus

```javascript
λx.x 
function (x) { return x; }


λx.λy.x
function (x, y) { return x; }


λf.λx.x
λf.λx.f x
λf.λx.f (f x)
```