---
title: "Notas en construcción"
layout: archive
permalink: /notas/borradores/
author_profile: false
classes: wide
entries_layout: grid
---

[Ordenar por temática](/notas/){: .btn .btn--inverse} 
[Ordenar por etiquetas](/notas/tags/){: .btn .btn--inverse} 
[Ordenar por fecha](/notas/fecha/){: .btn .btn--inverse} 
[Series monográficas](/notas/series){: .btn .btn--inverse}
[Borradores](/notas/borradores/){: .btn .btn--primary}

{% assign draft_posts = site.docs | where: "draft", true | sort %}
{% for post in draft_posts %}
    {% include archive-single.html %}
{% endfor %}
