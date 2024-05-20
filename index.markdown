---
layout: default
title: Home
---

## Blog Posts

{% for post in site.posts %}
  <article>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p><small>{{ post.date | date: "%B %d, %Y" }}</small></p>
    {{ post.content }}
  </article>
  <hr>
{% endfor %}
