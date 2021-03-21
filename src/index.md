---
title: My first page
layout: base.njk
---

Hello

{% for post in collections.book %}
  {{ post.data.title }}
  {{ post.url }}
  {{ post.data.date }}
  {{ post.data.tags }}
{% endfor %}