---
title: "Recursos"
layout: page
lang: pt
permalink: /recursos/
alt_lang: /en/resources/
show_title: false
exclude_from_listing: true
---

Os **Recursos** do Observatório Oceanográfico reúnem ferramentas, aplicações,
parsers e utilitários computacionais desenvolvidos para apoiar atividades de
pesquisa, extensão, ensino e análise de dados.

Diferentemente dos projetos institucionais, os recursos apresentados nesta
seção correspondem a **ferramentas reutilizáveis**, muitas vezes disponibilizadas
em código aberto, com documentação técnica mantida em plataformas externas,
como o GitHub.

---

{% assign resources = site.resources 
   | where: "lang", "pt" 
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


