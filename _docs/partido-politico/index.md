---
title: índice
layout: single
lastmod: 2024-07-06T13:40:53.451Z
---
{% assign pages = site.docs | where: 'label', 'partido-politico' %}

{% for page in pages %}
    <p><a href="{{page.url}}">{{page.title}}</href></p>
{% endfor %}