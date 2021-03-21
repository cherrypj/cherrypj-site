---
title: My first page
layout: base.njk
---

Hello

<ul>
{% for post in collections.book | reverse %}
  <li>{{ post.data.date }} <a href="{{ post.url}}">{{ post.data.title }}</a> {{ post.data.tags }}</li>
{% endfor %}
</ul>