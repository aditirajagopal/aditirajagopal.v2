---
layout: page
title: Blog
excerpt: "An archive of blog posts sorted by date."
search_omit: true
---

<ul class="post-list">
{% for post in site.categories.blog %} 
  <li><article><a href="{{ site.url }}{{ post.url }}" style="color:#66cccc;">{{ post.title }}</a><br><span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</article></li>
{% endfor %}
</ul>