---
layout: default
---

# Welcome

[About](about.html)

<h1>Blog Posts</h1>
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}"><span style="font-size:2em;"> {{ post.title }}</span></a> 
      <span>{{ post.date | date: "%B %d, %Y" }}</span><br>
      {{post.description}}
    </li>
  {% endfor %}
</ul>
