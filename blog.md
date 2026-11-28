---
title: Index
nav_order: 1
---
Cette documentation présente l'installation et l'utilisation du projet.

**Présentation.** Le projet fournit une bibliothèque simple, sans dépendance.
Un environnement récent et un éditeur de texte suffisent.

<ul>
  {% for post in site.posts | sort: "date" | reverse %}
    <li style="list-style:none;">
      <h2 id="{{ post.title | slugify }}" style="text-decoration:none;">{{ post.title }}</h2>
      {{ post.excerpt }}<a href="{{ post.url }}">via</a>
    </li>
  {% endfor %}
</ul>
