---
layout: default
---

{% for post in site.posts %}
<div style="margin: 20px 0; text-align: center;">
  <a href="{{ post.url | relative_url }}" style="text-decoration: none; letter-spacing: 1px; color: inherit;">
    {{ post.title }}
  </a>
</div>
{% endfor %}
