---
layout: single
---

{{ content }}

 {% assign reviewsInYear = site.posts | where_exp: "post", "post.type == libros" | group_by_exp: 'post', 'post.date | date: "%Y"' %}

<span class="total_count">Total anotaciones: {{ reviewsInYear | size }}</span>

<ul class="taxonomy__index">
  
  {% for year in reviewsInYear %}
    <li>
      <a href="#{{ year.name }}">
        <strong>{{ year.name }}</strong> <span class="taxonomy__count">{{ year.items | size }}</span>
      </a>
    </li>
  {% endfor %}
</ul>

  <div class="posts">

  {% assign list = site.data.books | where_exp: "review", "review" %}

  {% for year in reviewsInYear %}
  <section id="{{ year.name }}" class="taxonomy__section">
    <h2 class="archive__subtitle">{{ year.name }}</h2>
    <div class="entries-{{ entries_layout }}">

    {% for review in year.items %}
      {% for book in list %}
          {% if review.isbn and book.isbn and review.isbn == book.isbn %}
            {% include book-review.html %}
          {% endif %}
      {% endfor %}
    {% endfor %}
      </div>
    <a href="#page-title" class="back-to-top">{{ site.data.ui-text[site.locale].back_to_top | default: 'Back to Top' }} &uarr;</a>
  </section><br>
  {% endfor %}

 </div>
