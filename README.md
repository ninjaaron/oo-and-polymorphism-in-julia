# Object Orientation and Polymorphism in Julia

Contents:

- [Introduction](README.md)
- [Composition and Encapsulation](./comp-and-encap.ipynb)
- [Polymorphism and Code Reuse](./polymorphism.ipynb)

Please open an issue if anything doesn't make sense! I tried to be clear

## Introduction

[Julia](https://julialang.org/) is a language about which many
misconceptions abound. The worst one is that it's a language for
scientific computing, which isn't quite true. It's more like a
programming language designed to meet the needs of scientists--which
includes numeric computing, but also includes a wide range of
non-numeric tasks. I am not a scientist and rarely crunch numbers, but
I still find Julia applicable to many of the problems I'm interested
in.

However, another serious misconception is that Julia is *not* object
oriented. In fact, Julia is *more object oriented than Java*. You may
say, "Surely you jest, for everything is encapsulated in classes in
Java. Julia doesn't even *have* classes!"

Yes, Java has trained people to think that object oriented means "all
code is inside class bodies". However, this is completely false. Java
didn't invent object orientation, it co-opted it. Alan Kay, the
creator of Smalltalk coined the term object oriented to describe what
he was trying to do. Is all code inside of class bodies in Smalltalk?
No. You don't have to declare any classes if you're satisfied with
those that are already available to you. What makes Smalltalk purely
object oriented is that *everything is an object*. i.e. a first-class
value that can be passed around and has its own methods.

Here's a short list of some things that aren't objects in Java:

- types/classes
- methods
- source code
- primitives (can be passed around, but don't have methods).

Here are some things that are objects in Julia:

- types
- functions
- source code (and compiler-generated code)
- primitives
- everything else besides macros
  - (The whole point of macros is that they are resolved at
    compile-time, so it's kind of pointless to have them as runtime
    objects.)

Java takes a useful feature of Smalltalk, classes, and makes *that*
paradigmatic for the language, rather than the much more powerful idea
that all language elements are objects. Java forces the *programmer*
to design in an object-oriented way, but doesn't take OO as
paradigmatic for its own feature set. Smalltalk makes sure that
everything truely is an object, but allows programmers the freedom to
use simpler procedural or functional approaches to programming for
their own code.

Julia is object oriented in the latter sense.

Now, Java is not a bad language and supports (or enforces) object
oriented design for user code very well. However, you can use object
oriented design in almost any language, though it may not always be
ideal. For me, there are two central features of object orientation:

- data composition: the ability to create a new object that contains
  other objects.
- encapsulation: the ability to create a simple, flat interface to
  objects that are complex interenally.

Julia has excellent support for these design strategies. The one thing
it lacks is that there is no enforcement of *data hiding* in its
approach encapsulation. I used to think this data hiding wasn't
important, but I've changed my mind. It will be discussed later.

This tutorial is about how to use object oriented design patterns in
Julia, as well as its capabilities for polymorphism, such as multiple
dispatch, inheritance, generics, the trait pattern, etc. [Let's get on
with it, then](./comp-and-encap.ipynb).
