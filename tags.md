{% for tag in site.tags %} {{ tag[0] }} {% endfor %}
{% for tag in site.tags %}
{{ tag[0] }}
{% for post in tag[1] %}
{{ post.date | date:"%Y-%m-%d" }} {{ post.title }}
{% endfor %} {% endfor %}
