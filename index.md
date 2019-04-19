## Welcome to GitHub Pages

<form style="margin-bottom:10px;"><input type="text" placeholder="search.."></form>

<hr/>
{% for post in site.posts %}
  *   <span><!-- | {{ post.date | date_to_string }} --></span> » [{{ post.title }}]({{ post.url }} "{{ post.title }}")
{% endfor %}



<hr/>
{% for page in site.pages %}
  *   » [{{ page.title }}]({{ page.url }} "{{ page.title }}")
{% endfor %}

<hr/>
[Blog](./blog/index.html)
[About](about.md)
