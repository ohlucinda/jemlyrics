---
layout: default
---

{% for post in site.posts %}
  <p style="margin: 40px 0; text-align: center;">
    <a href="{{ post.url | relative_url }}" style="font-size: 22px; letter-spacing: 1px;">
      {{ post.title }}
    </a>
  </p>
{% endfor %}
