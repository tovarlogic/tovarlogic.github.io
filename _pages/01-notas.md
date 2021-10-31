---
title: "Notas breves"
breadcrumb_name: Notas
layout: archive
permalink: /notas/
classes: wide
entries_layout: grid
type: note
excerpt: "Sección donde recojo brevemente pensamientos que quiero recordar para más adelante desarrollarlos en un artículo."
last_modified_at: 2021-05-13
---

Mediante este `Libro de Notas` pretendo ir recogiendo todos los pensamientos que merecen ser recordados para más adelante reflexionar sobre ellos y desarrollar ideas. 

## Libro de notas

[Ordenar por temática](/notas/){: .btn .btn--inverse} 
[Ordenar por etiquetas](/notas/tags/){: .btn .btn--inverse} 
[Ordenar por fecha](/notas/fecha/){: .btn .btn--inverse} 
[Series monográficas](/notas/series){: .btn .btn--inverse}
[Borradores](/notas/borradores/){: .btn .btn--primary}

  {% assign items = site.docs | where: "doc_type", note %}
  {% for post in items %}
    {% include archive-single.html %}
  {% endfor %}

