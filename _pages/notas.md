---
permalink: /notas/
title: "Colección de recursos online"
last_modified_at: 2021-06-03
toc: true
toc_sticky: true
---

{% assign notes = site.docs.notas %}

{% for note in notes %}
## {{ note.title }}

{% endfor %}