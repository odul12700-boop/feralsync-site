---
layout: default
title: Actualités
description: "Veille biohacking, décryptages d'études et nouveautés FeralSync."
permalink: /actualites/
---

# Actualités

Veille, décryptages et nouveautés — publiés au fil de l'eau.

<ul class="post-list">
{% for post in site.posts %}
  <li>
    <p class="post-date">{{ post.date | date: "%d/%m/%Y" }}</p>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    {% if post.excerpt %}<p class="post-excerpt">{{ post.excerpt | strip_html | truncate: 160 }}</p>{% endif %}
  </li>
{% endfor %}
</ul>

{% if site.posts.size == 0 %}
<p><em>Les premiers articles arrivent bientôt.</em></p>
{% endif %}
