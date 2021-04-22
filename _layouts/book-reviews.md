---
layout: single_left
---

  <div class="posts">
  
  {% assign reviews = site.book_reviews | sort: "date" | reverse %}
  {% for review in reviews %}
  	{% include book-review.html %}
  {% endfor %}

 </div>
