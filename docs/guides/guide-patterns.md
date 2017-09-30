# Carefully use Patterns

## Introduction

Using the right pattern are very important. 

- MVP, MVC
- Command
- Observer
- Composite

and so on.

If you choose the right simple patterns they can you help to keep your application in order. If you choose the wrong pattern you get a complicated application and perhaps end up in a mess.

`**Choose wisely.**`

The first book from Gang-of-Four is very good.

## Solution

Find a good example. You can google for a pattern like MVP and find good example. Study them and play around with some sample application and if you really understand it and use it in your application.
If you do not understand do not use it. You get into a mess.

## Problem

Some patterns can bring your application down.
Some did not understand the pattern and misuse the pattern and did not do by a good example. So I saw a MVP pattern without a model. The Presenter was there but most of the code was in the View logic. The interface of the view was not filled. And in this case it would be better to use the old way instead of using a good pattern (MVC, MVP, ...) the wrong way.


## Notes: Criticism

http://wiki.c2.com/?PatternsAreNotTheLesserOfTwoEvils

Significant criticism has been directed at the concept of software design patterns generally, and at Design Patterns specifically.

A primary criticism of Design Patterns is that its patterns are simply workarounds for missing features in C++, replacing elegant abstract features with lengthy concrete patterns, essentially becoming a "human compiler" or "generating by hand the expansions of some macro".[4] Peter Norvig demonstrates that 16 out of the 23 patterns in Design Patterns are simplified or eliminated (via direct language support) in Lisp or Dylan.[5] Related observations were made by Hannemann and Kiczales who implemented several of the 23 design patterns using an aspect-oriented programming language (AspectJ) and showed that code-level dependencies were removed from the implementations of 17 of the 23 design patterns and that aspect-oriented programming could simplify the implementations of design patterns.[6]

Paul Graham wrote:

When I see patterns in my programs, I consider it a sign of trouble. The shape of a program should reflect only the problem it needs to solve. Any other regularity in the code is a sign, to me at least, that I'm using abstractions that aren't powerful enough-- often that I'm generating by hand the expansions of some macro that I need to write.

There has also been humorous criticism, such as a show trial at OOPSLA '99 on 3 November 1999,[7][8][a] and a parody of the format, by Jim Coplien, entitled "Kansas City Air Conditioner".