---
layout: default
title: Lyrics
---

{% for post in site.posts %}
  <p><a href="{{ post.url }}">{{ post.title }}</a></p>
{% endfor %}
