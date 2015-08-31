---
title: Danny Cheung
index_tags:
  - cheat sheet
  - docker
  - vagrant
  - python
  - ruby
  - jekyll
---

{% for t in page.index_tags %}
  {% for p in site.pages %}
    {% for page_tag in p.tags  %}
      {% if page_tag == t %}
        {% assign  page_count = page_count | plus: 1 %}
        {% if page_count == 1 %}
# {{ t | capitalize }}
<ul>
        {% endif %}
  <li><a href="{{p.url}}">{{p.title}}</a></li>
      {% endif %}
    {% endfor %}
  {% endfor %}
  {% if page_count > 0 %}
</ul>
  {% endif %}
  {% assign page_count = 0 %}
{% endfor %}
