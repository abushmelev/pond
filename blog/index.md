---
layout: page
title: Дневник прудика 
excerpt: "Жизнь прудика день за днем, сезон за сезоном, год за годом"
search_omit: true
image:
  feature: pond-title-white-lily.jpg
---

<ul class="post-list">
{% for post in site.categories.blog %} 
  <li><article><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
