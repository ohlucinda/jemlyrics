---
layout: default
---

{% for post in site.posts %}
<div>
<a href="{{ post.url | relative_url }}">{{ post.title }}</a>
</div>
{% endfor %}
