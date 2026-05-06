---
layout: default
title: Blog
permalink: /blog/
---

<div class="page-header">
  <p class="eyebrow">Blog</p>
  <h1>Research Notes & Articles</h1>
  <p class="lead">
    Short research articles, technical notes, conference reflections, and policy-oriented explainers.
  </p>
</div>

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <p class="post-meta">{{ post.date | date: "%B %-d, %Y" }}{% if post.categories %} · {{ post.categories | join: ", " }}{% endif %}</p>
      <p>{{ post.excerpt | strip_html | truncatewords: 35 }}</p>
    </li>
  {% endfor %}
</ul>
