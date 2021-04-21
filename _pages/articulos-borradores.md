---
title: "Borradores sin terminar"
breadcrumb_name: Borradores
layout: archive
permalink: /borradores/
author_profile: false
classes: wide
entries_layout: grid
---

{% assign draft_posts = site.posts | where: "draft", true | sort %}
{% for post in draft_posts %}
    {% include archive-single.html %}
{% endfor %}
