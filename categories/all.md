---
layout: single
permalink: /categories/
title: Categories
---

{% for category in site.categories %}
{% capture category_name %}{{ category | first }}{% endcapture %}
# {{ category_name }}
{% for post in site.categories[category_name] %}
- [{{ post.title }}]({{ site.baseurl }}{{ post.url }})
{% endfor %}
{% endfor %}
