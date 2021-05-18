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
  {% endfor %}
</ul>

  <div class="posts">
  
  {% assign reviews = site.book_reviews | sort: "date" | reverse %}

  {% assign list = site.data.books.list %}

  {% for review in reviews %}
    {% for book in list %}
        {% if review.isbn == book.isbn or review.olid == book.olid %}
          {% include book-review.html %}
          {% break %} {% break %}
        {% endif %}
    {% endfor %}
  {% endfor %}

 </div>
