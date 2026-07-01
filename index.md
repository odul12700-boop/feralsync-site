---
layout: default
title: Accueil
description: "FeralSync — biohacking, chronobiologie et hygiène de vie. Comprendre son corps pour mieux organiser son quotidien."
---

# Reprendre la main sur son hygiène de vie

**FeralSync**, c'est une conviction simple : le corps est une mécanique de précision.
Plutôt que de subir son quotidien, on peut l'organiser avec attention — lumière,
sommeil, alimentation, rythme. Pas de promesse miracle, pas de régime magique :
de la compréhension, des repères, et des outils.

<a class="btn" href="{{ '/application/' | relative_url }}">Découvrir l'application</a>
<a class="btn btn-secondary" href="{{ '/biohacking/' | relative_url }}">Comprendre le biohacking</a>

<div class="card">
<h2>⚙️ Les Intrants</h2>
<p>Une alimentation de qualité comme fondation, et des compléments choisis en
conscience pour la soutenir — jamais pour la remplacer.</p>
</div>

<div class="card">
<h2>🎛️ Les Paramètres</h2>
<p>Lumière du matin, couvre-feu des écrans, température de la chambre : les
signaux qui aident l'horloge interne à se caler entre éveil et repos.</p>
</div>

<div class="card">
<h2>🔄 Les Cycles</h2>
<p>Le jeûne comme temps de pause, le sommeil comme pilier de la récupération :
respecter les rythmes plutôt que les combattre.</p>
</div>

## Dernières actualités

<ul class="post-list">
{% for post in site.posts limit: 3 %}
  <li>
    <p class="post-date">{{ post.date | date: "%d/%m/%Y" }}</p>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    {% if post.excerpt %}<p class="post-excerpt">{{ post.excerpt | strip_html | truncate: 140 }}</p>{% endif %}
  </li>
{% endfor %}
</ul>

<a href="{{ '/actualites/' | relative_url }}">Toutes les actualités →</a>
