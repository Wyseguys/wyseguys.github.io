---
title: The First Age
header: true
age: 1
date: 2008-12-31 23:59:59
---
<div class="row">
  {% assign sorted = site.ashley | sort: 'date' %}
  {% for item in sorted %}
    {% assign is_header = item.header %}
    {% if is_header %}
    {% else %}
        {% if page.age == item.age %}
        <div class="col-md-3">
            <img src="{{ item.thumb }}" alt="{{ item.title }} gallery" />
            <a class="nav-link{% if item.url == page.url %} active{% endif %}" href="{{ item.url }}">{{ item.title }}</a>
        </div>
        {% endif %}
    {% endif %}
  {% endfor %}
</div>