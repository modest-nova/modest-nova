---
layout: default
title: Home
---

## 日報

{% for post in site.posts %}
  <article>
    <p><small>{{ post.date | date: "%Y/%M/%D" }}</small></p>
    {{ post.content }}
  </article>
{% endfor %}
