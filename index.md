---
layout: default
title:  Home
---
# Technical Tests
<ul>
{% for page in site.pages %}
  {% if page.layout == 'test' %}
  <li>
    <a href="{{ page.url }}">{{ page.title }}</a>
  </li>
  {% endif %}
{% endfor %}
</ul>
