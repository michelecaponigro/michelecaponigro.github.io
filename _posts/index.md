---
title: "Blog"
layout: default
permalink: /blog/
---
# Blog Posts

{% for post in site.posts %}
- [**{{ post.title }}**]({{ post.permalink }}) ({{ post.date | date: "%Y-%m-%d" }})
  {{ post.excerpt }}
{% endfor %}
