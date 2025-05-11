---
title: Home
layout: default
---

# Welcome to the Ultimate Band Archive

## Albums:

<ul>
{% for album in site.albums %}
  <li><a href="{{ site.baseurl }}{{ album.url }}">{{ album.title }}</a> ({{ album.year }})</li>
{% endfor %}
</ul>

# umm
{% for album in site.albums %}
  <p>{{ site.baseurl }}{{ album.url }}</p>
{% endfor %}