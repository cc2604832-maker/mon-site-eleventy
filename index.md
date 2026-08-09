---
layout: layout.njk
title: Bienvenue sur notre Boutique
---

<div class="grid">
{% for item in collections.produit %}
  <div class="card">
    <img src="{{ item.data.image }}" alt="{{ item.data.title }}">
    <h2>{{ item.data.title }}</h2>
    <div class="price">{{ item.data.prix }}</div>
    <a href="{{ item.url }}" class="btn">Voir le produit</a>
  </div>
{% endfor %}
</div>
