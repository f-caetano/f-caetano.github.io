---
layout: page
title: Archive
permalink: /archive/
---

## All articles

<ul class="archive-list">
{% for post in site.posts %}
  <li>
    <strong><a href="{{ post.url | relative_url }}">{{ post.title }}</a></strong><br>
    <span class="post-meta">{{ post.date | date: "%d %b %Y" }}</span><br>
    <span>{{ post.excerpt | strip_html | truncate: 160 }}</span>
  </li>
{% endfor %}
</ul>
``
