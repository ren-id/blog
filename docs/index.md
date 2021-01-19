{% include logo.html %}

# Stories

{% for post in site.posts limit:20 %}
1. [{{ post.title }}]({{ site.url }}{{ post.url }})
{% endfor %}

{% include link.html %}
