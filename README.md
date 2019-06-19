# Object Orientation and Polymorphism in Julia

Contents:

- [Introduction](README.md)
- [Composition and Encapsulation](./comp-and-encap.ipynb)
- [Polymorphism and Code Reuse](./polymorphism.ipynb)

Please open an issue if anything doesn't make sense! I tried to be clear

## Introduction

While [Julia](https://julialang.org/) is a purely object oriented
language in in same sense as Smalltalk--i.e. everything is an object--
Julia does lack some features in traditional object oriented languages;
namely, classes. However, Julia does have robust features that allow
many familiar patterns and strategies for abstracting complex data.

I like to think of object oriented programming not as bound to any
particular language features, but a set of approaches to data
abstraction that can be applied in virtually any general-purpose
programming language. These are the fundamental features required for an
OO approach to complexity, as I see them.

- data composition: the ability to create a new object that contains
  other objects.
- encapsulation: the ability to create a simple, flat interface to
  objects that are complex interenally.
- polymorphism: the ability to treat different objects of the different
  type similarly if they provide the same interfaces. (Kind of the bonus
  one.)

Classical object orientation puts all these features into classes.
Julia doesn't have classes, but does have features which provided
excellent support for these design strategies: stucts, methods, multiple
dispatch and flexible generics.

This tutorial is about how to use these features for data abstraction in
Julia, with some thoughts and comparisons about how they are similar to
and different from other languages. [Let's get on with it,
then](./comp-and-encap.ipynb).
