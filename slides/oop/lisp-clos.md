### CLOS 

The Common Lisp Object System

```
(defstruct point x y z)

(defun distance-from-origin (point)
  (let* ((x (point-x point))
         (y (point-y point))
         (z (point-z point)))
    (sqrt (+ (* x x) (* y y) (* z z)))))

(setf my-point (make-point :x 3 :y 4 :z 12))

(distance-from-origin my-point)
;;; 13.0
```