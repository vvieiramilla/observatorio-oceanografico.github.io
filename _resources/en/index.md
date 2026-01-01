---
title: "Resources"
layout: page
lang: en
permalink: /en/resources/
alt_lang: /recursos/
show_title: false
exclude_from_listing: true
---

The **Resources** section of the Oceanographic Observatory brings together
tools, applications, parsers, and computational utilities developed to support
research, outreach, teaching, and data analysis activities.

Unlike institutional projects, the resources presented here correspond to
**reusable tools**, often released as open-source software, with technical
documentation maintained on external platforms such as GitHub.

---

{% assign resources = site.resources 
   | where: "lang", "en" 
   | where_exp: "item", "item.exclude_from_listing != true" %}

<div class="entries-grid">
  {% for resource in resources %}
    <article class="entry resource-card">

      <a href="{{ resource.url | relative_url }}" class="resource-link">

        {% if resource.header.teaser %}
          <img src="{{ resource.header.teaser | relative_url }}"
               alt="{{ resource.title }}">
        {% endif %}

        <h3>{{ resource.title }}</h3>

      </a>

      {%- comment -%}
      {% if resource.resource_type %}
        <p class="resource-type">
          {{ resource.resource_type | capitalize }}
        </p>
      {% endif %}
      {%- endcomment -%}

    </article>
  {% endfor %}
</div>

