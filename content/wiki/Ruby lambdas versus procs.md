---
tags: ruby
---

Lambdas:

-   written using `lambda {}` syntax
-   check passed-in arguments against the arity of the block (in Ruby &gt;= 1.9)
-   `return` returns from the lambda

Procs:

-   written using `proc {}` or `Proc.new {}` syntax
-   do not check passed-in arguments against the arity of the block
-   `return` returns from the enclosing scope
