# Overview

Monad is pattern that amplify existing types with a new feature/aspect/expressiveness. Example is Nullable, Lazy, Future.
The Monad pattern is implemented by 2 basic operations/functions.

* `unit`: unit is one argument function of a type and return an amplified type called monadic type.
* `bind`: is 2 argument function. The first one is a monadic type, the second is a function of an underlying type (of the monadic type) and return other monadic type.

The 2 functions must satisfy 3 monad laws

1. `bind(unit(x), unit) == unit(x)` while `x` is variable of the underlying type
2. `bind(unit(x), f) == f(x)` while `f` is a function returning monadic type
3. `bind(unit(x),compose(f,g)) == bind(f(x),g)` while `compose` creates a function by apply `f` then `bind` of the result and `g`

References

* http://ericlippert.com/category/monads/
