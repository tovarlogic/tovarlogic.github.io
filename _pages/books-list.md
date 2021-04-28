---
title: "Listado con anotaciones de libros que he leido"
breadcrumb_name: Libros
taxonomy: Libros
layout: single_left
entries_layout: grid
classes: wide
author_profile: false
permalink: /libros/  
---
{% assign entries_layout = page.entries_layout | default: 'list' %}

{% assign readInYear = site.data.books.list | group_by_exp: 'same_year', 'same_year.date | date: "%Y"' | sort: "date" %}
{% assign reading = site.data.books.leyendo %}
{% assign pending = site.data.books.pendientes %}

[Todos los libros]({{ page.permalink }}){: .btn .btn--primary} [Solo con notas](/{{ page.taxonomy | downcase }}/reviews/){: .btn .btn--inverse}



