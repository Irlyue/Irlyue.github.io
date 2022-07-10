---
layout: single
permalink: /categories/
title: Categories
---

{% for category in site.categories %}
# {% capture category_name %}{{ category | first }}{% endcapture %}
{% for post in site.categories[category_name] %}
- [{{ post.url }}]({{ site.baseurl }}{{ post.url }})
{% endfor %}
{% endfor %}
