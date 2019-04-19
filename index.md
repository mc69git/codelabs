## Welcome to GitHub Pages

<form><input type="text" placeholder="search.."></form>
<hr/>
{% for post in site.posts %}
  *   <!-- <span>{{ post.date | date_to_string }}</span> --> » [{{ post.title }}]({{ post.url }} "{{ post.title }}")
{% endfor %}
<hr/>

[About](about.md)
