---
layout: layout.njk
title: Accueil - Mes Articles
---

Bienvenue sur mon site ! Voici la liste de mes derniers articles :

<ul>
{% for post in collections.post %}
  <li><a href="{{ post.url }}">{{ post.data.title }}</a> - {{ post.date | date: "%Y-%m-%d" }}</li>
{% endfor %}
</ul>
