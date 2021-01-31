{% for post in site.pages limit:10 %}
1. {{ post.title }}
{% endfor %}

{% for page in site.pages %}
{% if page.layout != nil %}
{% if page.layout != 'feed' %}
- {{ site.url }}{{ page.url | remove: 'index.html' }}
{% endif %}
{% endif %}
{% endfor %}
