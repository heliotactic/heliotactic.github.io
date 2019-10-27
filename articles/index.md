---
layout: page
title: Diffraction Experiments - attending to light and entanglements of measure and values
excerpt: "Archive of entangled thinking sorted by date."
search_omit: true
---

<ul class="post-list">
{% for post in site.categories.articles %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%d %B, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTcwMTI5OTAyN119
-->