---
title: ren, just ren | home
description: Aku tidak memposting di media sosial. Semua pemikiranku kutulis di sini.
---
# Stories

{% for post in site.categories.stories limit:20 %}
1. [{{ post.title }}]({{ site.url }}{{ post.url }})
{% endfor %}

# Tales

{% for post in site.categories.tales limit:20 %}
1. [{{ post.title }}]({{ site.url }}{{ post.url }})
{% endfor %}
