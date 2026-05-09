---
layout: default
title: Research Notes
permalink: /research-notes/
---

<section class="page-shell narrow">
  <div class="page-header"><p class="eyebrow">Research Notes</p><h1>Research Notes & Articles</h1><p class="lead">Short research articles, technical notes, conference reflections, and policy-oriented explainers.</p></div>
  <ul class="post-list">
    {% for post in site.posts %}
      <li class="post-card"><a href="{{ post.url | relative_url }}"><h3>{{ post.title }}</h3></a><p class="meta">{{ post.date | date: "%B %-d, %Y" }}{% if post.categories %} · {{ post.categories | join: ", " }}{% endif %}</p><p>{{ post.excerpt | strip_html | truncatewords: 35 }}</p></li>
    {% endfor %}
  </ul>
</section>
