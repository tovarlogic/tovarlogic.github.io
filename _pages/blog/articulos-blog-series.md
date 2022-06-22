---
title: "Blog: Series monográficas"
breadcrumb_name: series
layout: archive
permalink: /blog/series/
author_profile: false
classes: wide
entries_layout: grid
lastmod: 2022-06-17T11:42:06.043Z
---

[Ordenar por tipología y temática](/blog/){: .btn .btn--inverse} 
[Ordenar por etiquetas](/blog/tags/){: .btn .btn--inverse} 
[Ordenar por fecha](/blog/fecha){: .btn .btn--inverse}
[Series monográficas](/blog/series){: .btn .btn--primary}
[Borradores](/blog/borradores/){: .btn .btn--inverse}

{% assign series = site.posts | where: "serie_index", true | sort %}
{% for post in series %}
    {% include archive-single-serie.html type=entries_layout %}
{% endfor %}
