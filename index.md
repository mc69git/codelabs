## Welcome to GitHub Pages

<form style="margin-bottom:10px;"><input type="text" placeholder="search.."></form>

<hr/>
{% for post in site.posts %}
  *   <span>{{ post.url }} | {{ post.date | date_to_string }}</span> » [{{ post.title }}]({{ post.url }} "{{ post.title }}")
{% endfor %}
<hr/>


{% for page in site.collections.legal.docs %}
  *   <span>{{ post.title }} | {{ post.date | date_to_string }}</span> » [{{ post.title }}]({{ post.url }} "{{ post.title }}")
{% endfor %}

<hr/>
[Blog](./blog/index.html)
[About](about.md)
