---
layout: default
title: Home
---

## Blog Posts

{% for post in site.posts %}
  <article>
    <h2>{{ post.title }}</h2>
    <p><small>{{ post.date | date: "%B %d, %Y" }}</small></p>
    {{ post.content }}
  </article>
  <hr>
{% endfor %}
