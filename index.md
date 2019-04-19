## Welcome to GitHub Pages

<form style="margin-bottom:10px;"><input type="text" placeholder="search.."></form>

<hr/>
{% for post in site.posts %}
  *   <span>{{ post.url }} | {{ post.date | date_to_string }}</span> » [{{ post.title }}]({{ post.url }} "{{ post.title }}")
{% endfor %}
<hr/>

[About](about.md)
