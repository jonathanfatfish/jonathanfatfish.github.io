---
layout: page
# The tab name on the sidebar.
title: Daily Robotics News
icon: fas fa-robot
order: 1
---

## Daily Robotics News

A daily, source-linked digest of frontier robotics research and market demand signals.

{% assign digest_posts = site.posts | where_exp: "p", "p.categories contains 'Digest'" %}
{% assign en_posts = digest_posts | where_exp: "p", "p.tags contains 'en'" %}

{% assign latest_en = en_posts | first %}

### Today

<div class="d-flex flex-wrap gap-2 my-3">
  {% if latest_en %}
  <a class="btn btn-primary" href="{{ latest_en.url | relative_url }}">Today’s Digest</a>
  {% else %}
  <span class="btn btn-primary disabled">Today’s Digest (no post)</span>
  {% endif %}
</div>

<p class="text-muted mb-4">
  Latest: {% if latest_en %}<a href="{{ latest_en.url | relative_url }}">{{ latest_en.title }}</a>{% else %}(none){% endif %}
</p>

---

### Latest

{% for post in en_posts limit: 30 %}
- {{ post.date | date: "%Y-%m-%d" }} — [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}

> Tip: Use the search bar (top) to find a date or a topic quickly.
