---
title: Categories
layout: page
---

{% for category in site.categories %}
  <h3 id="{{ category[0] }}">{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
