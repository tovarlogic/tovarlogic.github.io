---
layout: single_left
---

{{ content }}

 {% assign reviewsInYear = site.book_reviews | where_exp: "item", "item.hidden != true" | group_by_exp: 'review', 'review.date | date: "%Y"' %}

<span class="total_count">Total anotaciones: {{ reviewsInYear | size }}</span>

<ul class="taxonomy__index">
  
  {% for year in reviewsInYear %}
    <li>
      <a href="#{{ year.name }}">
        <strong>{{ year.name }}</strong> <span class="taxonomy__count">{{ year.items | size }}</span>
      </a>
    </li>
    year
    {{ year }}
  {% endfor %}
</ul>

  <div class="posts">

  {% assign list = site.data.books.list | where_exp: "review", "review" %}

  {% for reviews in reviewsInYear %}
    {% for review in reviews %}
      {% for book in list %}
          {% if review.isbn and book.isbn and review.isbn == book.isbn %}
            {% include book-review.html %}
          {% endif %}
      {% endfor %}
    {% endfor %}
  {% endfor %}

 </div>
