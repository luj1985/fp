### Haskell High order function examples

```haskell
map (*2) [0,1,2,3,4,5,6]
-- [0,2,4,6,8,10,12]

filter (>3) [1,5,3,2,1,6,4,3,2,1] 
-- [5,6,4] 

foldr (+) 0 [1,2,3]
-- 6

let f = sqrt . abs
f (-100)
-- 10.0
```
