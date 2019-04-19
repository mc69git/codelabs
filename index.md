## Welcome to GitHub Pages

### Post
[Post](post.md)

<hr/>

{% for post in site.posts %}
  *   <span>{{ post.date | date_to_string }}</span> » [{{ post.title }}]({{ post.url }} "{{ post.title }}")
{% endfor %}
