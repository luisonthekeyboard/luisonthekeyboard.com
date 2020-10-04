---
layout: post
title: "The sum of a list of numbers"
date: "2015-01-02"
---

When trying to explain the difference between functional programming languages and imperative languages, one of the examples people usually give is the sum of a list of numbers.

Someone will say, for example, that in Haskell the sum of a list of numbers can be calculated like this:

```
    sum [1..10]
```

And the thesis is normally that this is much simpler and more elegant than doing a for loop, like so:

```
    in sum = 0;
    for(int x=1; x define a variable to keep my count and another variable for an iterator; now iterate over all the numbers from 1 to 10 and for each of them add it to the count variable. at the end of the loop, the result is in the count variable.
```

And that's the difference between `sum [1..10]` and the `sum(range(1,10))`.
