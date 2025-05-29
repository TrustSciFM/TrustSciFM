---
layout: page
title: blog
permalink: /blog/
description: A simple whitespace theme for academics. Based on [*folio](https://github.com/bogoli/-folio) design.
nav: false
nav_order: 6
---

# Blog Posts

{% for post in site.posts %}

<div class="post-preview">
  <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
  <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
  <p>{{ post.excerpt }}</p>
</div>
{% endfor %}
