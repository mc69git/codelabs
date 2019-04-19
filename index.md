---
title: Index..
---

## CodeLabs GitHub Pages

author:            Mehdi Chou.
summary:           CodeLab Tool
id:                codelab
categories:        tools
environments:      dev
status:            tutorial
feedback link:     github.com/mc69git

<div class="blurb">

# Hi there, I'm MC!

[tuto!](post.md)

</div>

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> » <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
