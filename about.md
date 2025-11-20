---
layout: default
title: About
description: Sascha – pathways between creativity and business.
permalink: /about/
---
<section class="about-section">
  <div class="about-container">
    <h1 class="about-title">About Me</h1>

    <div class="about-grid">
      <div class="photo-card">
        <img src="https://northlightpath.com/images/NPL.png" alt="Sascha - North Light Path">
      </div>

      <div class="cards-column">
        <div class="info-card">
          <h2>Who I Am</h2>
          <p>I'm a systems-minded creative with a background in business leadership, project operations, and team design. Over the past several years, I've led initiatives across technology, process, and people building teams, managing multimillion-dollar budgets, and shaping how collaboration and clarity take root in complex environments.</p>
          <p>These days, I’m focused on contract work and completing my first poetry manuscript, <em>Weigh Station: Notes from the Quiet Years</em>—a collection tracing the quiet transformations between identity, belonging, and voice.</p>
        </div>

        <div class="info-card">
          <h2>About This Site</h2>
          <p>North Light Path is a living résumé—part portfolio, part experiment—written in HTML, CSS, JavaScript, and a little AI to keep curiosity alive. It’s a space where planning meets play, where systems and imagination coexist without the need for order.</p>
        </div>
      </div>
    </div>

    <!--  3-latest-posts section  -->
    <div class="info-card" style="margin-top:3rem">
      <h2>Recent Notes</h2>
      <div class="blog-preview">
        {% for post in site.posts limit:3 %}
          <article>
            <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
            <time>{{ post.date | date: "%b %d, %Y" }}</time>
            <p>{{ post.excerpt | strip_html | truncatewords:20 }}</p>
          </article>
        {% endfor %}
        <p><a href="{{ '/blog' | relative_url }}">All notes →</a></p>
      </div>
    </div>

  </div>
</section>
