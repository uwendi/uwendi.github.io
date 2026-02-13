---
layout: default
title: Research & Archives
permalink: /research/
---

# Research & Archives

This section is for longer-form material and preserved work:
- reconstructed and translated thesis excerpts
- research notes
- older writing I want to curate and republish

---

## Ongoing Series

### Reconstructed Master’s Thesis (2005–2007)

A reconstructed, translated, and lightly annotated edition of my Master’s thesis on the formal verification of graph algorithms (DFS and BFS).

Each chapter is published as a separate post, with educational notes and present-day commentary.

{% raw %}
<ul>
  {% assign thesis_posts = site.categories["masters-thesis"] | sort: "date" | reverse %}
  {% for post in thesis_posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <small> — {{ post.date | date: "%Y-%m-%d" }}</small>
    </li>
  {% endfor %}
</ul>
{% endraw %}
