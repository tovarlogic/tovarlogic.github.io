---
permalink: /recursos/
title: "Colección de recursos online"
last_modified_at: 2021-06-03
toc: true
toc_sticky: true
---

{% assign bookmarks = site.data.bookmarks.raindrop %}

{% for bookmark in bookmarks %}
## {{ bookmark.title }}
<iframe style="border: 0; width: 100%; height: 450px;" allowfullscreen frameborder="0" src="https://raindrop.io/tovarlogic/{{ bookmark.id }}/embed"></iframe>
{% endfor %}