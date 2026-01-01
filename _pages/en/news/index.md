---
layout: page
title: News
lang: en
permalink: /en/news/
alt_lang: /noticias/
---

<h1 class="hero-title">News</h1>
<h2 class="hero-subtitle">Updates, events, and activities from the Observatório Oceanográfico</h2>

<div class="news-list">
  {% for post in site.posts %}
    {% if post.lang == "en" %}
      <article class="news-item">
        <h3>
          <a href="{{ site.baseurl }}{{ post.url }}">
            {{ post.title }}
          </a>
        </h3>
        <p class="news-meta">
          {{ post.date | date: "%B %d, %Y" }}
        </p>
        {% if post.excerpt %}
          <p>{{ post.excerpt }}</p>
        {% endif %}
      </article>
    {% endif %}
  {% endfor %}
</div>
