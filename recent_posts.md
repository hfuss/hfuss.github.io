---
title: recent.posts
layout: default
---

<ul>
  {% for post in site.posts limit: 20 %}
    <li><a href="{{ post.url }}">{{ post.date | date: "%m-%d-%Y" }} - {{ post.title }}</a></li>
  {% endfor %}
</ul>