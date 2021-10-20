---
layout: default
title: Notes
permalink: /notas/
entries_layout: grid
---

[Ordenar por etiquetas](/notas/){: .btn .btn--primary} 
[Ordenar por fecha](/notas/fecha/){: .btn .btn--inverse} 

<h1>Staff</h1>

<ul>
  {% for note in site.notes %}
    <li>
      <h2><a href="{{ note.url }}">{{ note.title }}</a></h2>
    </li>
  {% endfor %}
</ul>