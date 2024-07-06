---
title: índice
layout: single
permalink: partido-politico/
lastmod: 2024-07-06T13:52:14.849Z
---
{% assign docs = site.docs | where: 'label', 'partido-politico' %}

{% for file in docs %}
    <p><a href="{{file.url}}">{{file.title}}</href></p>
{% endfor %}