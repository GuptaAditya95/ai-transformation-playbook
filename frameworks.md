---
layout: page
title: Frameworks
permalink: /frameworks/
---

Every framework from the course, in one place.

<ul class="framework-list">
{% for post in site.posts %}{% if post.framework %}
  <li>
    <a class="fw-name" href="{{ post.url | relative_url }}">{{ post.framework }}</a><br>
    {{ post.summary }}
  </li>
{% endif %}{% endfor %}
</ul>
