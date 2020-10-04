---
layout: post
title: "It's gophers all the way down..."
date: "2016-10-23"
---

I have learned many programming languages since I started playing with computers. Some I have learned because of my work but the majority during my time at University and because of my curiosity.

I guess this is the reason why I never saw myself as a one language man -- curiosity drives me to experiment and play, and I'm constantly very aware of the many things I don't know; and because of that (and the utterly clever people who continue to create new languages) there's always a next language to learn.

This has happened to me during my whole professional life but I started documenting it more recently. Here's the languages I've learned and played with per year, excluding whatever I'm using at my day job ([first](https://tomtom.com) it was Java, [then](https://here.com) Javascript, [now](https://redpineapplemedia.com) Clojure):

- 2012 -- Clojure
- 2013 -- Ruby, Scheme
- 2014 -- R, Scala
- 2015 -- Haskell, Clojure

During this whole time, I've learned a lot about learning new languages. I've learned about [what exercises to try](https://projecteuler.net/archives), what [code challenges to do](https://www.hackerrank.com/), how to evaluate several different parts of learning a language, from testing to package management, from editor support to documentation. Since every year I play with one or two new languages, I end up repeating the same initial workflows.

Lately I've been thinking that I'm missing a more mainstream general purpose language.

I wouldn't like to go back to Java, since the purpose is to learn something new. I know I won't learn C++ because I'm just not that clever, really. And while Haskell, Clojure and Scala are certainly general-purpose, I have found (thanks to [my job at Red Pineapple Media](https://www.linkedin.com/in/decomputed/)) that finding jobs (or candidates) with those skills is not at all trivial. The [Python Paradox](http://www.paulgraham.com/pypar.html) is true -- people wth these skills are certainly special, but the amount of jobs is low (in comparison, obviously), the amount of companies wanting to bet on those technologies is not high, and one needs a more general skill to be marketable.

So I started with this list:

- Rust
- Go
- Python
- Perl
- Kotlin
- C

And used the following constraints to narrow it down

- A language which was not too esoteric (no functional languages or lisps);
- Compiled;
- Which could be lower-level than VM-based languages
- With a small core
- Statically typed
- Not necessarily object-oriented

Kotlin looks super nice, a very elegant middle ground between Java and Scala. But I really wanted to move away from the JVM.

Perl, unfortunately, seems to be dying a very slow death.

Python is one of those things (like shell scripting) which I think I should know, I feel like I have an obligation of knowing it, but it's interpreted and eventually not going to be very fast.

Go has pretty much all the points. However, it is garbage-collected, and I wouldn't mind to go back to (manual) memory management. It is also a bit plagued with many very odd choices (no generics, no package management, no libreary versioning, ...) and so it seems more like a Google tool that was made public rather than something with a strong future.

Rust also has all the points, with some bonuses (such as it allowing some FP patterns and having a really nice type system). However it is very very young, still very imature and I wonder how much low-level it really is.

Finally, C. C has been probably the language I have enjoyed the most in my life. It would certainly be super interesting to get back to it but I'm not sure how sensible it is to invest now in a 44 year-old language, which has not evolved as fast as it should have.

So, I had 3 contenders: Go, Rust and C.

C was easy to discard, since I wouldn't be learning anything new.

Rust is, in theory, my favorite choice. But since it is very imature, I think it would be hard to get proficient in it. It is still too soon to see how the general public will react to the memory management concepts Rust introduces, it may end up being too esoteric for the general public.

Go, it turns out, is my favorite in practice. It is very very fast to get into Go, the things it is missing are being handled by the community and there are quite a few very large projects already written in Go, which gives me some confidence in the language.

After seeing videos by the Go team, the concepts and principles really resonated with me. The criticisms have been well received by the team and there is openness about handling not only Generics but also package management.

After trying Go, it felt very natural to get back to an imperative, mutable language. Perhaps because of knowing the drawbacks and perils of mutability I found myself changing memory regions by pointer and being very aware about what I was doing. The type system, while not very advanced, it is ... good enough.

Having Google behind it and seeing how much they have been listening to the community gives me some hope that it will evolve in the right direction.

So with all of this in my mind, Go is my new general purpose language, and the next language I want to invest the most in.

"And you, young Rust; we shall watch your career with great interest." :-)
