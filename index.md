---
layout: default
title: Home
permalink: /
---

<div class="hero-card">
  <div class="hero-eyebrow">Filipe Caetano</div>
  <h1 class="hero-title">TROUBLESHOOTING SOMETHING… </h1>
  <p class="hero-subtitle">
    Maybe Fabric? Power BI? Or something that AI is there yet
  </p>
</div>

<h2 class="section-title">Articles</h2>

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
    The blog is my small attempt to leave behind some information I wish I knew before.
    <i>No affiliation, it reflects only my own opinions, notes, and personal views</i>.
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
