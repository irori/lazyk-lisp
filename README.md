LazyK-Lisp
==========

A toy Lisp interpreter in Lazy K.

How to Use
----------

    $ lazyk lisp.lazy
    > (car '(a b c))
    a
    > (cdr '(a b c))
    (b c)
    > (cons 1 (cons 2 (cons 3 ())))
    (1 2 3)
    > (defun fact (n) (if (eq n 0) 1 (* n (fact (- n 1)))))
    fact
    > (fact 8)
    40320
    > (defun fib (n) (if (eq n 1) 1 (if (eq n 0) 1 (+ (fib (- n 1)) (fib (- n 2))))))
    fib
    > (fib 10)
    89
    > (set 'count 0)
    0
    > (defun incr () (set 'count (+ count 1)))
    incr
    > (incr)
    1
    > (incr)
    2
    > (incr)
    3

Builtin Functions
-----------------

- car
- cdr
- cons
- eq (can compare numbers)
- atom
- +, -, *, /, mod
- set

Special Forms
-------------

- quote
- if
- lambda
- defun

Links
-----

- [The Lazy K Programming Language](http://homepages.cwi.nl/~tromp/cl/lazy-k.html)
- [Lazy K interpreter](https://github.com/irori/lazyk)
- [Online Lazy K interpreter](http://lazy-k.appspot.com/)
