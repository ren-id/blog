<h1>Kisah</h1>
<ol>
{% for post in site.pages limit:10 %}
<li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ol>
