---
layout: default
title: Home
permalink: /
---

<div class="hero-card">
  <div class="hero-eyebrow">Troubleshooting notes from the virtual side</div>
  <h1 class="hero-title">TROUBLESHOOTING SOMETHING… POWER BI? Fabric? Or maybe what AI cannot capture <u>YET</u></h1>
  <p class="hero-subtitle">
    A minimal, modern, human-first technical blog for edge cases, product quirks, field lessons, and practical escalation notes.
  </p>
</div>

<h2 class="section-title">Latest articles</h2>

<div class="card-grid">
  {% for post in site.posts limit:3 %}
    <article class="post-card">
      <div class="post-card-meta">
        <span class="badge">{{ post.categories | first | default: "notes" }}</span>
        {{ post.date | date: "%d %b %Y" }}
      </div>
      <h3 class="post-card-title">
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h3>
      <div class="post-card-excerpt">
        {{ post.excerpt | strip_html | truncate: 180 }}
      </div>
      <a href="{{ post.url | relative_url }}">Read article →</a>
    </article>
  {% endfor %}
</div>

<div class="soft-panel" style="margin-top: 32px;">
  <h2 style="margin-top: 0;">Why this blog?</h2>
  <p>
    When working with data, it is only a matter of time until you hit something a bit more unique:
    a strange business requirement, a production issue, an undocumented limitation, or a behavior that
    does not quite fit what the glossy overview promised.
  </p>
  <p>
    This blog is my small attempt to leave behind the kind of page I wish I had found faster:
    practical, searchable, and hopefully useful at least one time.
  </p>
</div>

<div class="soft-panel" style="margin-top: 22px;">
  <h2 style="margin-top: 0;">Main topics</h2>
  <div class="topic-list">
    <span class="topic-pill">Power BI / Fabric</span>
    <span class="topic-pill">SQL Server / SSRS</span>
    <span class="topic-pill">Paginated Reports</span>
    <span class="topic-pill">Tabular Models / AAS</span>
    <span class="topic-pill">DAX / T-SQL</span>
    <span class="topic-pill">Microsoft Azure</span>
  </div>
</div>
