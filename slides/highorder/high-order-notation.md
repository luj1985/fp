```
map :: (a -> b) -> [a] -> [b]
reduce / foldr :: (a -> b -> b) -> b -> [a] -> b
filter ::  (a -> Bool) -> [a] -> [a]
compose :: (b -> c) -> (a -> b) -> a -> c
```