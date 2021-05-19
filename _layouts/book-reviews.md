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

  {% assign list = site.data.books.list | where:'review' %}
  list
  {{ list }}
  {% for review in reviewsInYear %}
  review.items
  {{ review.items }}
    {% for book in list %}
        {% if review.isbn == book.isbn %}
          {% include book-review.html %}
        {% endif %}
    {% endfor %}
  {% endfor %}

 </div>
