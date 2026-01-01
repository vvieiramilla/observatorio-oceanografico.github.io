---
title: "Portfólio"
layout: page
lang: en
alt_lang: /portfolio/
permalink: /en/portfolio/
---

{% assign projects = site.projects | where: "lang", "en" %}

<div class="project-list">
  {% for project in projects %}
    <article class="project-card">
      {% if project.header.teaser %}
        <div class="project-thumb">
          <img src="{{ project.header.teaser | relative_url }}"
               alt="{{ project.title }}">
        </div>
      {% endif %}

      <div class="project-body">
        <h3 class="project-title">
          <a href="{{ project.url | relative_url }}">{{ project.title }}</a>
        </h3>

        <p class="project-excerpt">
          {{ project.excerpt }}
        </p>

        <a class="project-link" href="{{ project.url | relative_url }}">
          Learn more →
        </a>
      </div>
    </article>
  {% endfor %}
</div>
