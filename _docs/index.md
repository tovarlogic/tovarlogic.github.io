---
title: Índice de documentos (bloc de notas)
layout: single
permalink: /docs/
lastmod: 2024-07-06T13:51:19.349Z
---
{% assign docs = site.docs %}
{% assign collections = site.collections %}

{{ collections }}

{% for doc in docs %}
    <p><a href="{{doc.url}}">{{doc.title}}</href></p>
{% endfor %}