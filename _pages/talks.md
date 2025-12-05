---
title: "Talks"
permalink: /talks/
layout: single
author_profile: true
---

## Conferenze e Presentazioni

### Talk Recenti
{% for post in site.talks reversed %}
  {% if forloop.index <= 5 %}
  - **{{ post.date | date: "%Y" }}:** {{ post.title }}  
    {{ post.venue }}, {{ post.location }}
  {% endif %}
{% endfor %}

### Archivio Completo
{% for post in site.talks reversed %}
  {% if forloop.index > 5 %}
  - **{{ post.date | date: "%Y" }}:** {{ post.title }}
  {% endif %}
{% endfor %}
