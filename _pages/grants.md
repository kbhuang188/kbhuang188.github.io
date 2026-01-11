---
layout: single
title: "Grants"
permalink: /grants/
---
<div class="grant-grid">
  {% for g in site.data.grants %}
  <div class="grant-card">
    <div class="grant-title">{{ g.title }}</div>
    <div class="grant-meta">
      <span class="grant-pill">{{ g.period }}</span>
      <span class="grant-pill">{{ g.sponsor }}</span>
      <span class="grant-pill">{{ g.role }}</span>
    </div>
    <div class="grant-tags">
      {% for t in g.tags %}
      <span class="grant-tag">{{ t }}</span>
      {% endfor %}
    </div>
    {% if g.link and g.link != "" %}
      <div class="grant-link"><a href="{{ g.link }}">Read more</a></div>
    {% endif %}
  </div>
  {% endfor %}
</div>
