---
title: ren, just ren | home
description: Aku tidak memposting di media sosial. Semua pemikiranku kutulis di sini.
---
{% include logo.html %}

# Stories

{% for post in site.posts limit:20 %}
1. [{{ post.title }}]({{ site.url }}{{ post.url }})
{% endfor %}

{% include link.html %}
