---
layout: post
title: How to solve bugs?
author: Vasiliy
categories: support
tags: [support, development, testing]
---

A framework for resolving issues you might encounter in a production
environment. It should allow you to solve most of the bugs in a system or
application.

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
in the system. Does it align with each other?

Of course, as the prerequisite of this step you need some level of
understanding of the solution. If you don't have it yet, read the corresponding
conceptual and functional documentation or ask teammates to transfer the
knowledge to you.

## Step 3. Try to reproduce in the test landscape

It is easy to fix reproduceable issues. If you are able to reproduce, you can
launch a debug session and understand what went wrong exactly.

Sometimes you can't reproduce the issue in the test system. Or you can
reproduce it, but only in a small number of cases. Those are the hardest ones
to solve.

### Step 3.1. Debug

If you were lucky to a reproduceable bug, the next step would be to use debug
environment to figure out what went wrong exactly. This is a kind of art on its
own, so I will not cover be able to cover it within this article.

Some general guidelines:


## Step 4. Look at the code

This doesn't give results as often as previous steps and requires some skill to
execute. However, for a skilled person it is easier than the next steps, so I
usually do it before going further.

What to look for:
1. **Logical mistakes**. These are easy to make and sometimes hard to
   catch.
	- `OR` instead of `AND`
	- `=` instead of `!=`
	- "Is initial instead" of "is not initial"
2. **Edge cases**. What if you will receive an empty input? What if object is
   locked or changed By another user or a previous action?
