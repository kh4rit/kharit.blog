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

<!-- citations below were done with
[jekyll-scholar](https://github.com/inukshuk/jekyll-scholar), but it is not
working with GitHub Pages, so I removed it -->
> Good Design Is Easier to Change Than Bad Design
> 
> [[1] (Thomas & Hunt, 2019)](#references)

A great feature from SAP systems is that they are designed to be changed. In
any software you can theoretically change the source code of the system, but a
good-designed system provides you with instruments to change them in a
controlled maner. These changes will not complicate system updates and
maintenance. SAP created special user exits (like BAdIs or Business Add-Ins),
that allow you to implement your business logic within a predefined framework.
Standard system expects you to write your custom code there and responds
correctly to it.

If you are an SAP consultant, you have to know and use those enhancement
options. You should know what is the difference between them, when to use the
one with syncronized processing or the one with asyncronized processing, when
to enhance the update, which one will show a log to a user, which one can be
restarted in case of user locks.

Independently if you are connected to SAP or not you can always apply the ETC
principle. You can use it as a metric to assess solution directions. Please
find below a couple of questions you might want to ask yourself during the
design process:

- A room with curved walls vs a regular squared one, --- which one is easier to
  change or repurpose?
- What colors will be good with any kind of furniture?
- Which method of taxation will give a company the most flexibility? Which one
  is possible to change later?

---

When we connect ETC principle to software engineering we should start thinking
in terms of solution that is more flexible and will live longer as a
consequence. The following guidelines are intended specifically for software
consultants:

1. **No misuse**. Use system documents and fields, configurations, interfaces
   and APIs, in the way the creator intended for. It might be tempting to solve
a problem quick and dirty by writing a value to an existing field (that is
intended for other purpuse, but is not currently used). Don't do it. It might
save some implementation time, but it will really complicate further
developments, support and maintenance.
2. **Write and update documentation**. This includes most importantly a
   Solution design concept, but also Development specifications. It might not
seem to be connected with ETC principle, however, imagine receiving from a
previous partner a system with zero documentation. How much harder will it be
to change and maintain a system without any documentation?
3. **Solve business requirements**, not functional or technical. It doesn't
   mean that you should ignore functional requirements, but it is important to
find a root cause behind them, --- the business requirement. If you don't
understand the business needs the chances that your solution will fit a
business process are quite small. Continue to dig untill business requirements
are crystal clear. And also, write them down. Ask stupid questions, be a little
annoying if needed.
4. **Look for a balance** between changing a business or changing a solution.
   If your solution is closer to standard, it is much easier to enhance and
maintain it. However, you can't make fully standard solutions as customers need
to differentiate themselves from the competition with their own advantages.
Practice to find the right balance.

References
----------
1. Thomas, D., & Hunt, A. (2019). *The Pragmatic Programmer, 20th Anniversary
   Edition*. Addison Wesley.
