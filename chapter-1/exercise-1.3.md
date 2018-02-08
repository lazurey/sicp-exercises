# Exercise 1.3
Define a procedure that takes three numbers as arguments and returns the sum of the squares of the two larger numbers.

## My answer
```lisp
(define (square x) (* x x))
(define (sum-of-larger-two-squares a b c)
  (cond ((and (> a b) (> b c)) (+ (square a) (square b)))
        ((and (> b a) (> c a)) (+ (square b) (square c)))
        (else (+ (square a) (square c)))
  )
)
```

## Standard answers
[sicp community](http://community.schemewiki.org/?sicp-ex-1.3)
