---
layout: blog
title: Home
section: Home

feed: atom.xml
keywords: Blog, Programming, Software, Development
---

My Thoughts On ...
==========================================

Software. Sustainability. Startups.

Recent Posts
------------

{% for post in site.categories.blog limit:5 %}
<div class="section list">
  <h1>{{ post.date | date_to_string }}</h1>
  <p class="line">
  <a class="title" href="{{ post.url }}">{{ post.title }}</a>
  <a class="comments" href="{{ post.url }}#disqus_thread">View Comments</a>
  </p>
  <p class="excerpt">{{ post.excerpt }}</p>
</div>
{% endfor %}

<p>
<a href="/blog/past.html">Older Posts &rarr;</a>
</p>
