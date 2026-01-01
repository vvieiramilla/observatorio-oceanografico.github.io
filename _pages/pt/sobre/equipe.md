---
layout: page
title: Equipe
lang: pt
permalink: /sobre/equipe/
alt_lang: /en/about/team/
---

<h1 class="hero-title">Equipe</h1>

<div class="team-grid">

  {% assign people = site.people | where: "lang", "pt" | sort: "order" %}

  {% for person in people %}
    <a href="{{ site.baseurl }}{{ person.permalink }}" class="team-card">

      <img
        src="{{ site.baseurl }}{{ person.avatar }}"
        alt="{{ person.title }}"
        class="team-avatar"
      >

      <div class="team-meta">
        <strong class="team-name">{{ person.title }}</strong>

        {% if person.role %}
          <span class="team-role">{{ person.role }}</span>
        {% endif %}
      </div>

    </a>
  {% endfor %}

</div>

<hr>

<p class="alumni-link">
  <a href="{{ site.baseurl }}/sobre/alumni/">
    → Alumni do Observatório Oceanográfico (ex-integrantes)
  </a>
</p>


