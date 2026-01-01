---
layout: page
title: Notícias
lang: pt
permalink: /noticias/
alt_lang: /en/news/
---

<h1 class="hero-title">Notícias</h1>
<h2 class="hero-subtitle">Atualizações, eventos e atividades do Observatório Oceanográfico</h2>

<div class="news-list">
  {% for post in site.posts %}
    {% if post.lang == "pt" %}
      <article class="news-item">
        <h3>
          <a href="{{ site.baseurl }}{{ post.url }}">
            {{ post.title }}
          </a>
        </h3>
        <p class="news-meta">
          {{ post.date | date: "%d/%m/%Y" }}
        </p>
        {% if post.excerpt %}
          <p>{{ post.excerpt }}</p>
        {% endif %}
      </article>
    {% endif %}
  {% endfor %}
</div>
