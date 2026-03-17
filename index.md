---
layout: default
title: Lyrics
---

{% for post in site.posts %}
<a href="{{ post.url | relative_url }}">{{ post.title }}</a>

{% endfor %}
