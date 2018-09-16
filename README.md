# Home page

Welcome to Vasiliy Kharitonov's personal blog.

You can use the links below to navigate to recent posts.

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
