---
permalink: /recursos-online/
title: Colección de recursos online
last_modified_at: 2021-06-03
toc: true
toc_sticky: true
comments: false
lastmod: 2022-06-01T13:01:46.711Z
---

{% assign categories = site.data.categories.bookmarks %}

<div class="card">
    <div class="card-header pb-2 d-flex justify-content-between align-items-start">
        <span class="d-inline">
            <button class="btn btn-sm btn-primary" id="new-item" style=""><i class="fas fa-fw fa-plus"></i> Dejar un comentario</button>
        </span>
    </div>
    <div class="card-body">
        {% include forms/bookmark-form.html %}      
    </div>
</div>

{% for category in categories %}

    {% assign bookmarks = site.data.bookmarks %}

    {% if bookmarks.size > 0 %}
        ## {{ category[1] }}
        {% for bookmark in bookmarks %}
            - [{{ bookmark.title}}]({{ bookmark.url}})  
        {% endfor %}
    {% endif %}

{% endfor %}