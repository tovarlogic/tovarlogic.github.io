---
title: índice
layout: single
lastmod: 2024-07-06T13:38:19.266Z
---
{% assign pages = site.docs | where: 'label', 'linux'}

{% for page in pages %}
    <p><a href="{{page.url}}">{{page.title}}</href></p>
{% endfor %}