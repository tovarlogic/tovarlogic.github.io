---
layout: single_left
---

{{ content }}

<span class="total_count">Total anotaciones: {{ reviewsInYear | size }}</span>

<ul class="taxonomy__index">
  {% assign reviewsInYear = site.book_reviews | where_exp: "item", "item.hidden != true" | group_by_exp: 'review', 'review.date | date: "%Y"' %}
  
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
  {% assign lists = site.data.books.lists %}

  {% for review in reviews %}
    {% for list in lists %}
      {% for book in list %}
        {{ book }}
        {% if review.isbn == book.isbn or review.olid == book.olid %}
          {% include book-review.html %}
        {% endif %}
      {% endfor %}
    {% endfor %}
  {% endfor %}

 </div>
