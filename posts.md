---
layout: default
title: Posts
permalink: /posts/
---

# Posts

{% if site.posts.size == 0 %}
_This is where blog posts will live. No posts yet — coming gradually._
{% else %}
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <small> — {{ post.date | date: "%Y-%m-%d" }}</small>
    </li>
  {% endfor %}
</ul>
{% endif %}
