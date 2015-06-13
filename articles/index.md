---
layout: page
title: Околопрудные записи
excerpt: "Заметки на тему пруда и все что вокруг него"
search_omit: true
image:
  feature: pond-title-nimphea.jpg
---

<ul class="post-list">
{% for post in site.categories.articles %} 
  <li><article><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
