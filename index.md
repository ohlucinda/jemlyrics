---
layout: default
---

{% for post in site.posts %}
  <p style="margin-bottom: 20px;">
    <a href="{{ post.url | relative_url }}">
      {{ post.title }}
    </a>
  </p>
{% endfor %}
