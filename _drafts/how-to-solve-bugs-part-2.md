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
