---
layout: page
title: notes
permalink: /blog/
nav: true
nav_order: 4
pagination:
  enabled: true
---

<div class="post">
  <header class="post-header">
    <h1 class="post-title">{{ site.blog_name }}</h1>
    <p class="post-description">{{ site.blog_description }}</p>
  </header>

  <ul class="post-list">
    {% if page.pagination.enabled %}
      {% assign postlist = paginator.posts %}
    {% else %}
      {% assign postlist = site.posts %}
    {% endif %}
    {% for post in postlist %}
    <li>
      <h3><a class="post-title" href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p>{{ post.description }}</p>
      <p class="post-meta">{{ post.date | date: '%B %d, %Y' }}</p>
    </li>
    {% endfor %}
  </ul>
  {% if page.pagination.enabled %}{% include pagination.liquid %}{% endif %}
</div>
