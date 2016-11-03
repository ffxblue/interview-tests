---
layout: default
title:  Home
---
# Technical Tests
<ul>
{% for page in site.pages %}
  {% if page.layout == 'test' %}
  <li>
    <a href="{{ site.baseurl }}{{ page.url }}">{{ page.title }}</a>
  </li>
  {% endif %}
{% endfor %}
</ul>
