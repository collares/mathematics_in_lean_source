.. _sets_and_functions:

Sets and Functions
==================

The vocabulary of sets, relations, and functions provides a uniform
language for carrying out constructions in all the branches of
mathematics.
Since functions and relations can be defined in terms of sets,
axiomatic set theory can be used as a foundation for mathematics.

Lean's foundation is based instead on the primitive notion of a *type*,
and it includes ways of defining functions between types.
Every expression in Lean has a type:
there are natural numbers, real numbers, functions from reals to reals,
groups, vector spaces, and so on.
Some expressions *are* types,
which is to say,
their type is ``Type``.
Lean and mathlib provide ways of defining new types,
and ways of defining objects of those types.

Conceptually, you can think of a type as just a set of objects.
Requiring every object to have a type has some advantages.
For example, it makes it possible to overload notation like ``+``,
and it sometimes makes input less verbose
because Lean can infer a lot of information from
an object's type.
The type system also enables Lean to flag errors when you
apply a function to the wrong number of arguments,
or apply a function to arguments of the wrong type.

Lean's library does define elementary set-theoretic notions.
In contrast to set theory,
in Lean a set is always a set of objects of some type,
such as a set natural numbers or a set of functions
from real numbers to real numbers.
The distinction between types and set takes some getting used to,
but this chapter will take you through the essentials.
