---
layout: page
title: 'An Extensible Dynamically-Typed Hierarchy of Exceptions'
description: ""
category: publications
tags: []
---
(Simon Marlow) *Haskell '06: Proceedings of the 2006 ACM SIGPLAN workshop on Haskell*, Portland, Oregon, ACM Press, September 2006

<a href="http://simonmar.github.io/bib/papers/ext-exceptions.pdf">Full Paper</a> | <a href="extexceptions06.bib">BibTeX</a>

In this paper we address the lack of extensibility of the exception
type in Haskell.  We propose a lightweight solution involving the use
of existential types and the Typeable class only, and show how our
solution allows a fully extensible hierarchy of exception types to be
declared, in which a single overloaded catch operator can be used to
catch either specific exception types, or exceptions belonging to any
subclass in the hierarchy.  We also show how to combine the existing
object-oriented framework OOHaskell with our design, such that
OOHaskell objects can be thrown and caught as exceptions, with full
support for implicit OOHaskell subtyping in the @catch@ operator.
