---
layout: post
title: "How I got into Haskell"
date: "2015-01-28"
---

It would only be fair to say that I actually started this whole thing with Clojure; last year, around April or May, when I spent 3 weeks of vacation learning Clojure, among other things. It was super productive time and I ended up with a [Markdown parser](https://github.com/decomputed/adamastor) and a [very small static blog engine](https://github.com/decomputed/bloguito).

I was already convinced of the motivation for Functional Programming (no state, no side effects, exploiting parallelism...) but I also wanted to know how other languages approached the paradigm.

Since Scala is the other big functional language in the JVM, that's what I went with next. Back in November Coursera started a Scala course with none other than Martin Odersky so I joined. The experience though wasn't as nice as with Clojure. I felt a constant struggle to stay away from the imperative mode of the language and started craving for something which would really lock me down in Functional mode. That was, after all, what I had enjoyed in Clojure - the language is very opionated.

So I started looking for an alternative again and that's how I got into Haskell. So how did I approached it then?

I started by listening to Simon Peyton Jones talking about [Being Lazy with Class](https://www.youtube.com/watch?v=7NPBrWDzO2A) and immediatelly got hooked. Haskell's history and Simon's pitch in that talk really convinced me that it was more important to learn the essentials, the core basics of FP in a pure and restricted environment.

After knowing the principles, it's all a matter of syntax.

So I bought [Programming in Haskell](http://www.cs.nott.ac.uk/~gmh/book.html) from Graham Hutton, and watched Erik Meijer's [talks on Channel 9](http://channel9.msdn.com/Series/C9-Lectures-Erik-Meijer-Functional-Programming-Fundamentals/), which are based on that same book, as well as a refreshment of those talks on eDX.

I think this was a fantastic way of being introduced to the language since I heard the talks, did the exercises, then read the chapter and did a few more exercises. And even though both Channel 9 and eDX talks had the same structure and were about the same topics, they were very different in style. Channel9's talks were a lot more technical; Erik goes to the whiteboard and explains code equivalents in other languages, draws things and explains the historical context of many of the ideas.

So about a month later, what's it like?

I think it's probably the environment where I was more productive sooner. Things just flow. The language has a very terse syntax and it becomes almost a direct correspondence between the thought structure and the code. No braces, no semi-colons, nothing. Just the code needed to solve the problem.

There's a really deep support for functional programming, and this was a revelation for me - supporting the functional paradigm is way more than just lambdas or lazy ranges: it's partial functions, and function composition and a default library which promotes this way of thinking. Anonymous functions a lá Java and Javascript just barely scratch the surface.

Static typing and type inference, which are one of the battle crys of Haskellists, are really helpful features. The compiler knows the type of everything you define and forces you to respect those types. And this essentially means that you don't ever ever need to write defensive code. A function that operates on Integers will never be used with Strings. Never. Ever. Which means I don't need to check for those cases. And that eliminates a lot of code which has nothing to do with the problem at hand.

In other words, I think I'm hooked. :-)
