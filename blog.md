---
layout: default
title: Blog
permalink: /blog/
---

<section class="about-section">
  <div class="about-container">
    <h1 class="about-title">Notes</h1>

    {% for post in site.posts %}
      <div class="info-card">
        <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
        <time>{{ post.date | date: "%b %d, %Y" }}</time>
        <p>{{ post.excerpt | strip_html | truncatewords:30 }}</p>
      </div>
    {% endfor %}

  </div>
</section>