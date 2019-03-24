---
title: The Second Age
header: true
age: 2
date: 2009-12-31 23:59:59
---
<div class="row">
  {% assign sorted = site.ashley | sort: 'date' %}
  {% for item in sorted %}
    {% assign is_header = item.header %}
    {% if is_header != true %}
        {% if page.age == item.age %}
        <div class="col-md-3 text-center">
            {% if item.thumb != null %}
              <a href="{{ item.url }}"><img src="{{ item.thumb }}" alt="{{ item.title }} gallery" class="rounded-circle"/></a>
              <a href="{{ item.url }}"><div><span class="badge badge-default text-wrap">{{ item.title }}</span></div></a>
            {% endif %}
            {% if item.thumb == null %}
              <a href="{{ item.url }}"><h3><span class="badge badge-default text-wrap">{{ item.title }}</span></h3></a>
            {% endif %}
        </div>
        {% endif %}
    {% endif %}
  {% endfor %}
</div>