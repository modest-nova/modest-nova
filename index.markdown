---
layout: default
title: Home
---

## Blog Posts

{% for post in site.posts %}
  <article>
    <p><small>{{ post.date | date: "%Y/%M/%D" }}</small></p>
    {{ post.content }}
  </article>
  <hr>
{% endfor %}
