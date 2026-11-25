---
title: Blog
nav_order: 1
---
Cette documentation présente l'installation et l'utilisation du projet.

**Présentation.** Le projet fournit une bibliothèque simple, sans dépendance.
Un environnement récent et un éditeur de texte suffisent.

<ul>
  {% for post in site.posts | sort: "date" | reverse %}
    <li style="list-style:none;">
      <h2 style="text-decoration:none;" id="{{ post.title | slugify }}"><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
