---
layout: default
title: Daily Curation
---

<h1>Daily Curation</h1>

<p>AI/ML papers, tech videos, and Hacker News picks — one digest per day.</p>

<ul>
{% for post in site.posts limit:60 %}
  <li><a href="{{ post.url }}">{{ post.title }}</a> — {{ post.date | date: "%b %d, %Y" }}</li>
{% endfor %}
</ul>