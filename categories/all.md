---
layout: single
permalink: /categories/
title: Categories
---

{% for category in site.categories %}
# {{ category_name }}
{% for post in site.categories[category_name] %}
- [{{ post.url }}]({{ site.baseurl }}{{ post.url }})
{% endfor %}
{% endfor %}
