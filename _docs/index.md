---
title: Índice de documentos (bloc de notas)
layout: single
permalink: /docs/
lastmod: 2024-07-06T13:55:13.148Z
---
{% assign docs = site.docs %}
{% assign collections = site.collections %}

{{ collections[0] }}
{{ collections[1] }}
{{ collections[2] }}

{% for doc in docs %}
    <p><a href="{{doc.url}}">{{doc.title}}</href></p>
{% endfor %}