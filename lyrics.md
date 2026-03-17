---
layout: default
---

{% for post in site.posts %}
<div style="margin: 12px 0; text-align: center;">
  <a href="{{ post.url | relative_url }}">
    {{ post.title }}
  </a>
</div>
{% endfor %}
