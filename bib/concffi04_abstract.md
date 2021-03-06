---
layout: page
title: 'Extending the {H}askell Foreign Function Interface with Concurrency'
description: ""
category: publications
tags: []
---
(Simon Marlow, Simon Peyton Jones, Wolfgang Thaller) *Proceedings of the ACM SIGPLAN workshop on Haskell*, pages 57--68, Snowbird, Utah, USA, September 2004

<a href="http://simonmar.github.io/bib/papers/conc-ffi.pdf">Full Paper</a> | <a href="concffi04.bib">BibTeX</a>

A Haskell system that includes both the Foreign Function Interface and
the Concurrent Haskell extension must consider how Concurrent Haskell
threads map to external Operating System threads for the purposes of
specifying in which thread a foreign call is made.

Many concurrent languages take the easy route and specify a one-to-one
correspondence between the language's own threads and external OS
threads.  However, OS threads tend to be expensive, so this choice can
limit the performance and scalability of the concurrent language.

The main contribution of this paper is a language design that provides
a neat solution to this problem, allowing the implementor of the
language enough flexibility to provide cheap lightweight threads,
while still providing the programmer with control over the mapping
between internal threads and external threads where necessary.
