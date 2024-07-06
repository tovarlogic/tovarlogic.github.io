---
title: índice
layout: single
permalink: /docs/linux/
lastmod: 2024-07-06T13:52:26.580Z
---

{% assign docs = site.docs | where: 'label', 'linux' %}

{% for file in docs %}
    <p><a href="{{file.url}}">{{file.title}}</href></p>
{% endfor %}