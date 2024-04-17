---
layout: default
---

# Welcome

[About](about.html)

<h1>Blog Posts</h1>

<hr>
{% for post in site.posts %}
  <span>{{ post.date | date: "%B %d, %Y" }}</span> <br>
  <a href="{{ post.url }}"><span style="font-size:2em;"> {{ post.title }}</span></a> <br>
  {{post.description}}
  <br>
  <hr>
{% endfor %}

