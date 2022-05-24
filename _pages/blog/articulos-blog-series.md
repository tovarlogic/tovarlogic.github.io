---
title: "Blog: Series monográficas"
breadcrumb_name: series
layout: archive
permalink: /blog/series/
author_profile: false
classes: wide
entries_layout: grid
lastmod: 2022-05-24T07:50:04.158Z
---

[Ordenar por tipología y temática](/blog/){: .btn .btn--inverse} 
[Ordenar por etiquetas](/blog/tags/){: .btn .btn--inverse} 
[Ordenar por fecha](/blog/fecha){: .btn .btn--inverse}
[Series monográficas](/blog/series){: .btn .btn--primary}
[Borradores](/blog/borradores/){: .btn .btn--inverse}

{% assign series_pages = site.pages | where: "item", "item.layout == series" | sort %}
{% for page in series_pages %}
    {% include archive-single.html %}
{% endfor %}
