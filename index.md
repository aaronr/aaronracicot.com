---
layout: page
title: 
---

![cover](public/images/cover.png)

{% assign pages_list = site.pages %}
{% for node in pages_list %}
  {% if node.title != null %}
    {% if node.layout == "page" %}
<a href="{{ node.url }}">{{ node.title }}</a> : {{ node.tagline }}
    {% endif %}
  {% endif %}
{% endfor %}

