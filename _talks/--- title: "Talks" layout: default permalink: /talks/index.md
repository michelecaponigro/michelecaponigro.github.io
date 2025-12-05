---
title: "Talks"
layout: default
permalink: /talks/
---
# My Talks
{% for talk in site.talks %}
  - [**{{ talk.title }}**]({{ talk.permalink }}) ({{ talk.date | date: "%Y-%m-%d" }}, {{ talk.venue }})
{% endfor %}
