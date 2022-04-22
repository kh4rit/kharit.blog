---
layout: post
title: The Essense of Good Design
author: Vasiliy
categories: consulting
tags: [the-pragmatic-consultant, consulting, design]
---

This post is a part of series [The Pragmatic Consultant](/tags/the-pragmatic-consultant).

---

**In the core of good design is the ETC (Easier To Change) principle.**

<!-- citations below are done with [jekyll-scholar](https://github.com/inukshuk/jekyll-scholar) -->
{% quote the-pragmatic-programmer %}
Good Design Is Easier to Change Than Bad Design
{% endquote %}

A great feature from SAP systems is that they design them to be changed. In any
software you can theoretically change the source code of the system, but a
good-designed system provides you with instruments to change them in a
controlled maner. These changes will not complicate system updates and
maintenance. SAP created special user exits (like BAdIs or Business Add-Ins),
that allow you to implement your business logic within a predefined framework.
Standard system expects you to write your custom code there and responds
correctly to it.

If you are an SAP consultant, you have to know and use those enhancement
options. You should know what is the difference between them, when to use the
one with syncronized or asyncronized processing, when to enhance the update,
which one will show a log to a user, which can be restarted in case of user
locks.

Independently if you are connected to SAP or not you can always apply the ETC
principle. You can use it as a metric to assess solution directions. Please
find below a couple of questions you might want to ask yourself during the
design process:

- A room with curved walls vs a regular squared one, --- which one is easier to
  change or repurpose?
- What colors will be good with any kind of furniture?
- Which method of taxation will give a company the most flexibility? Which one
  is possible to change later?

When we connect this principle to software engineering we 

References
----------
{% bibliography --cited_in_order %}
