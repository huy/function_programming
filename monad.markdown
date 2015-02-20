# Overview

Monad is pattern that amplify existing types with a new feature/aspect/expressiveness. Example is Nullable, Lazy, Future.
The Monad pattern is implemented by 2 basic operations/functions.

* unit: unit is one argument function of a type and return an amplified type called monadic type.
* bind: is 2 argument function. The first one is a monadic type, the second is a function of an underlying type (of the monadic type) and return other monadic type.

References

* http://ericlippert.com/category/monads/
