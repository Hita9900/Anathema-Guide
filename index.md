---
title: Home
layout: default
---

# Welcome to the Ultimate Band Archive

## Albums:

<ul>
{% for album in site.albums %}
  <li><a href="{{ album.url }}">{{ album.title }}</a> ({{ album.year }})</li>
{% endfor %}
</ul>
