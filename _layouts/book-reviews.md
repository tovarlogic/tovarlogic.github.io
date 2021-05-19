---
layout: single_left
---

{{ content }}

 {% assign reviewsInYear = site.book_reviews | where_exp: "item", "item.hidden != true" | group_by_exp: 'review', 'review.date | date: "%Y"' %}
 reviewsinYear
{{ reviewsInYear }}
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
  
  {% assign reviews = site.book_reviews | sort: "date" | reverse %}

  {% assign list = site.data.books.list %}

  lista
  {{ list }}
  {% for review in reviews %}
    {% for book in list %}
        {% if review.isbn contains book.isbn or review.olid contains book.olid %}
          {% include book-review.html %}
        {% endif %}
        book 
        {{ book }}
    {% endfor %}
    review.isbn 
    {{ review.isbn }}
  {% endfor %}

 </div>
