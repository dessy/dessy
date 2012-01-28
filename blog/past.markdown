---
layout: blog
title: Archives
section: Past

feed: atom.xml
keywords: Blog, Programming, Software, Development
---

Archives
========

This is the full list of all blog posts.

{% for post in site.categories.blog %}
<div class="section list">
  <h1>{{ post.date | date_to_string }}</h1>
  <p class="line">
  <a class="title" href="{{ post.url }}">{{ post.title }}</a>
  <a class="comments" href="{{ post.url }}#disqus_thread">View Comments</a>
  </p>
  <p class="excerpt">{{ post.excerpt }}</p>
</div>
{% endfor %}
