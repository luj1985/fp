### Haskell

nothing is evaluated until necessary

```haskell
-- if-else
g x y = (if x == 0 then 1 else sin x / x) * y
```


```haskell
-- read entire file
hGetContents :: Handle -> IO String

```