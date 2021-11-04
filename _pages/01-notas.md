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

Lo sencillo es expresar las ideas u opiniones de manera espontánea (que para eso es esta sección de "Notas", con independencia de lo elaborado y estenso del texto), lo complicado es informarse y realizar un estudio sobre cualquier asunto, para posteriormente articular un juicio basado en evidencias (para eso será a partir de ahora 1 de Nov de 2021 la sección de artículos del blog)

[Ordenar por temática](/notas/){: .btn .btn--inverse} 
[Ordenar por etiquetas](/notas/tags/){: .btn .btn--inverse} 
[Ordenar por fecha](/notas/fecha/){: .btn .btn--primary} 
[Series monográficas](/notas/series){: .btn .btn--inverse}
[Borradores](/notas/borradores/){: .btn .btn--inverse}

  {% assign items = site.docs | where: "doc_type","note" | sort: 'date' | reverse %}
  {% for post in items %}
    {% include archive-single.html type=entries_layout %}
  {% endfor %}

