---
title: "Notas breves"
breadcrumb_name: Notas
type: note
permalink: /notas/
excerpt: "Sección donde recojo brevemente pensamientos que quiero recordar para más adelante desarrollarlos en un artículo."
last_modified_at: 2021-05-13
---

Mediante este `Libro de Notas` pretendo ir recogiendo todos los pensamientos que merecen ser recordados para más adelante reflexionar sobre ellos y desarrollar ideas. 

## Libro de notas
<ul>
  {{ assign items = site.docs | where "doc_type", page.type }}
  {% for item in items %}
    <li>
      <h2><a href="{{ item.url }}">
      		{{ item.title }}
      	  </a>
      </h2>
    </li>
  {% endfor %}
</ul>