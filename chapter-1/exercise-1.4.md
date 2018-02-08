# Exercise 1.4
Observe that our model of evaluation allows for combinations whose operators are compound expressions. Use this observation to describe the behavior of the following procedure:
```
(define (a-plus-abs-b a b)
  ((if (> b 0) + -) a b))
```

## My answer
1. it defined a function called `a-plus-abs-b` and it accepts 2 parameters: `a` and `b`
2. if `b` is greater than `0`, then use `+`, otherwise use `-`
3. return `a + b` or `a - b`

## Standard answer
`a + |b|`
