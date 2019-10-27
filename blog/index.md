---
layout: page
title: "Queering Solar - Blogging traces of quantum entanglement"
excerpt: "Helio-Tactics and Seeds of Disruption: The Revolution will not be televised."
image:
  path: /images/NorthPorch_SC_2016.png
  credit: JRS Brownson

---

<ul class="post-list">
{% for post in site.categories.blog %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
