---
layout: default  # Specify the layout if needed
title: Blog
---

<h1>Blog</h1>

<ul class="post-list">
  {% for post in site.posts %}
    <li class="post-item">
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{ post.date | date: "%B %d, %Y" }}</p>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>
