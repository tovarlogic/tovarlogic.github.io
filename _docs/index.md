---
title: Índice de documentos (bloc de notas)
layout: single
lastmod: 2024-07-06T13:36:39.067Z
---
{% assign docs = site.docs %}
{% assign collections = site.collections %}

{{ collections }}

{% for doc in docs %}
    <p><a href="{{doc.url}}">{{doc.title}}</href></p>
{% endfor %}