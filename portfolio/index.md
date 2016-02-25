---
layout: page
title: Portfolio
excerpt: "An archive of projects I've worked on"
search_omit: true
---

<ul class="post-list">
{% for post in site.categories.portfolio %} 
  <li><article><a href="{{ site.url }}{{ post.url }}" style="color:#66cccc;">{{ post.title }}</a><br><span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</article></li>
{% endfor %}
</ul>