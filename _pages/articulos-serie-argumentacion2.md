---
permalink: /series/argumentacion2
serie: argumentacion
---

{% assign posts = site.posts | where: "serie", page.serie %}

<ul>

    {% for post in posts %}
    <li>
       <a href="{{ post.url }}">{{ post.title }}</a> | <span class="date">{{ post.date | date: '%d %b %Y' }}</span>
    </li>
    {% endfor %}

</ul>
