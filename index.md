---
title: Index
nav_order: 1
---
Cette documentation présente l'installation et l'utilisation du projet.

## Présentation
Le projet fournit une bibliothèque simple, sans dépendance.

## Prérequis
Un environnement récent et un éditeur de texte suffisent.

<ul style="list-style:none; margin:0; padding:0">
  {% for post in site.posts | sort: "date" | reverse %}
    <li>
      <p id="{{ post.title | slugify }}"><a href="{{ post.url }}">{{ post.title }}</a></p>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
