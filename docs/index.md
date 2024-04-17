---
layout: default
---

# Welcome

[About](about.html)

<h1>Blog Posts</h1>
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span>{{ post.date | date: "%B %d, %Y" }}</span>
      {{post.description}}
    </li>
  {% endfor %}
</ul>
