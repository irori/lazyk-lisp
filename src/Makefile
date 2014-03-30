# Path to hs2lazy (https://github.com/irori/hs2lazy)
HS2LAZY ?= hs2lazy

lisp.lazy: lisp.hs
	$(HS2LAZY) hs2lazy-prelude.hs lisp.hs >lisp.lazy

# Native compile
lisp: lisp.hs
	ghc lisp.hs
