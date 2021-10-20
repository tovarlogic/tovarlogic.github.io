---
layout: default
title: Staff
---
<h1>Staff</h1>

<ul>
  {% for note in site.notes %}
    <li>
      <h2>{{ note.title }}</h2>
      <p>{{ note.content | markdownify }}</p>
    </li>
  {% endfor %}
</ul>