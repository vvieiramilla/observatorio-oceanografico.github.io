---
layout: page
title: Team
lang: en
permalink: /en/about/team/
alt_lang: /sobre/equipe/
---

<h1 class="hero-title">Team</h1>

<div class="team-grid">

  {% assign people = site.people | where: "lang", "en" | sort: "order" %}

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
  <a href="{{ site.baseurl }}/en/about/alumni/">
    → O₂ Alumni (former members)
  </a>
</p>

