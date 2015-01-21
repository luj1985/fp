### Side effect in Pure FP langauge

Haskell Monad
```haskell
main :: IO ()
main =  do c <- getChar
           putChar c
```