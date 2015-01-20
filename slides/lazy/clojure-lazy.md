### Clojure

lazy-seq


```clojure
(defn positive-numbers 
  ([] (positive-numbers 1))
  ([n] (cons n (lazy-seq (positive-numbers (inc n))))))

;;; #'user/positive-numbers

(take 5 (positive-numbers))
;;; (1 2 3 4 5)
```