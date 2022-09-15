---
layout: post
title: Blogging for nerds --- Jekyll + GitHub + vim
author: Vasiliy
categories: blogging
tags: [jekyll, blogging, github, vim]
---
---

Don't you like the idea of having you own little platform to share your
thoughts and news curated by you?

Then my proposal would be to consider looking into Jekyll static blog generator
which is actually hosted by GitHub for free for you under the name of GitHub
Pages.

---

First of all, what is a static (blog) website generator? It is a very efficient
program that can help you manage content for your site. The main difference
from CMS like WordPress is it doesn't have a database, nor any dynamic
scripting --- all of the site content is saved as simple HTML pages. Static
website generators allow you to efficiently create and update these HTML pages. 

Let's say you want to add a link to a new page into a header menu for all of
the pages of your website. It will be a hassle to update all the HTML files
manually, so this is what a static website generator will do for you.

Another thing it takes care for is generating the HTML itself. It is not as
convinient to write an HTML document as it is to write a note in Markdown.
Jekyll allows you to automatically convert Markdown documents into HTML
documents.

Websites that are built using such generators are amazingly fast, --- there is
no additional processing needed per request, no delay upon receiving the
information from database. These websites are actually as fast as they go.

---

So, what do you need to get started? A couple of things:
- GitHub account.
- Your own domain (optional).
- Web browser.

That's all you need to get started!

---

To create your first website you can follow the instructions below:
1. Create a repository in GitHub for you website. If you don't have custom
   domain, you get one from GitHub for free. In this case create a repository
with the following name <your username>.github.io. Otherwise you can create it
with the domain name, e.g. example.com.
2. Create a file in the root of the repository `index.md`. Add there some
   information you would like to see on the home page of your website.
3. Activate environment GitHub Pages in the settings of your repository.

If you have a custom domain, you need to also set up DNS record for it.
Otherwise, Thats it! Really easy so far.

---

The next steps I suggest you to do is to set up your Jekyll, so you would be
able to build the website locally. It doesn't make sense to create a commit to
see a result of each small test you execute.
