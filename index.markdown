---
layout: default
title: Home
---

## 日報

{% for post in site.posts %}
  {% assign align_class = forloop.index | modulo: 2 | prepend: 'align-' %}
  <article class="{{ align_class }}">
    <h2>{{ post.title }}</h2>
    <p><small>{{ post.date | date: "%Y/%m/%d" }}</small></p>
    {{ post.content }}
  </article>
{% endfor %}
