---
layout: post
title: How to solve bugs? Part 1
author: Vasiliy
categories: support
tags: [support, development, testing]
---

A framework for resolving issues you might encounter in a production
environment. It should allow you to solve most of the bugs in a system or
application. This is the Part 1.

## Step 1. Listen to users

When you already have some experience it is tempting to dismiss information
that users provide to you about the problem. You might think: this is waste of
time, they lack IT skills to understand the problem, you know better. However,
this is not the right thing to do because of many reasons.

As the first step it is good to undestand in details what is the problem the
users complain about. If you have an incident number or description --- read it
carefully, -- it might save you time in future.

Of course it is possible that there is no bug at all, it is a missing feature
or a user mistake, this first step usually allows you to determine it.

## Step 2. Look at the data

In good designed systems and applications you have documents and logs to
analyse. Check the data, try to understand what was going on,
what might went wrong.

If it is not immediately obvious, try to collect more examples, good and bad,
look for similarities between them.

Try to map the information users provided about the bug with the data you have
in the system. Does it match?

Of course, as a prerequisite of this step you need some level of understanding
of the solution. If you don't have it yet, read the corresponding conceptual
and functional documentation or ask team members to transfer the knowledge to
you.

## Step 3. Try to reproduce in the test landscape

It is easy to fix reproduceable issues. If you are able to reproduce, you can
launch a debug session and understand what went wrong exactly.

Sometimes you can't reproduce the issue in the test system. Or you can
reproduce it, but not reliably, only in a small number of cases. Those are the
hardest ones to solve.

### Step 3.1. Debug

If you were lucky to have a reproduceable bug, the next step would be to use
debug environment to figure out what went wrong exactly. This deserves an
article on its own, so I won't go into a lot of details here.

Some general guidelines:
- **Don't assume impossible**. It is always better to check to be completely sure.
- **Isolate the problem**. Split the program in 2, check which part causes it. Then
  split again and again. Eventually you should find a part that is causing the
  problem.
- **Use specialized software**. It might be tempting to just print some strings to
  a console and it even works most of the times. However, investing your time
  to learn debugging software is always better in long-term.
- **Don't dismiss a code that is not yours**. Pointing fingers will not help to
  solve the problem. Debugging someone else's code will.
- **Don't dismiss your own code either**. It is much more likely to find a bug in
  your own code, than in a library that is used by thousands of people.
- **Make notes**. When you debug a big program writing a note can help you to
  understand it better and faster.
- [**Talk to the duck**](https://en.wikipedia.org/wiki/Rubber_duck_debugging).
  Articulating a problem to someone else or even to an imaginary person like a
  rubber duck can help you solve the problem.

To be continued...
