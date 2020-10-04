---
layout: post
title: "First steps into Clojure"
date: "2012-08-25"
---

I've been looking for a new language to learn.

Javascript and Java are currently part of my job, so all the new things I have to learn in those languages I already learn them in my dayly job. Besides, they are quite mainstream and I wanted something a bit more exotic.

I peaked into Scala a couple of times already but I'm (still?) not convinced of the whole _scalable language_ concept. I feel like a small language, with few constructs, and then extended with itself, is something that appeals more to me.

Since I like the idea of staying in the JVM ecossystems, the other exotic option was [clojure](http://clojure.org "Clojure").

I studied Lisp in university and I enjoyed it a lot. I remember that my [friend Hubert](http://twitter.com/neotyk) was a big fan of Clojure. And since he was one of the few truly inspiring people with whom I worked at Tomtom, I guess I could just follow his lead on this one.

So, if you're just like me, thinking about how to start, I'll describe the general setup you'll want to have so that you can play with Clojure in two different ways:

- Using the REPL, a command line environment where you can just try clojure commands;
- Building a small application and run tests on it, like a maven project where I can have my code, my tests, build the project and have a deliverable at the end.

So here we go!

1. ([Leiningen](https://leiningen.org)) -- leiningen is the Clojure equivalent of Maven. And it integrates with Maven in such a beautiful way that it's just a relief. Get it the old-fashioned way since package managers are still using the older clojure 1.3.0;
2. So, since lein is like maven, it downloads whatever dependencies you may need, one of them being... Clojure. Its dependencies come from Clojars, the clojure equivalent to Maven Central, but also from maven central;
3. Now, it turns out that with lein you immediately have both the REPL and a way to create new project. To try the REPL just do `lein repl`;
4. To create a new project do `lein new awesome-project`. That is the equivalent to `mvn archetype:generate`, except it doesn't ask you for anything -- and creates a proper project.
5. With that project created, cd into its directory and try `lein test`, `lein clean`, `lein install`. `lein help` will give you a list of options you can use but the one that's really nice is `lein pom` -- it generates a `POM` file for your project, which means that you can now import it into IntelliJ;
6. [La Clojure](https://github.com/JetBrains/la-clojure "La Clojure @ github")) is the plugin you'll want to use if you use IntelliJ. Head over to intellij, open the plugins, search for clojure, choose La Clojure, install and restart. now import your project from the pom file you created above.

So, my first observation is that things just seem to work. _Batteries included_ kind of way.

You get leiningen and it is working without any configuration. You create a pom file and it's valid and intellij reads it. The project that was generated with `lein new` has a documentation folder with a doc written in [markdown](http://daringfireball.net/projects/markdown/ "Markdown").

The people behind this seem to follow this idea of "[convention over configuration](https://en.wikipedia.org/wiki/Convention_over_configuration "convention over configuration")" and that is so refreshing.

So the next step is to continue learning this.

Nothing is ever finished, it seems. :-)
