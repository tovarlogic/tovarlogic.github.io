---
layout: single_left
---
<div class="home">
	<div class="call-out"><h1>Book Reviews</h1>
	    Here are notes I've taken on books I've read. Some are in-depth, some are short, some include quotes. I've included ratings and genres for future sorting.
	</div>
  <div class="posts">
  
  {% assign reviews = site.book_reviews | sort: "date" | reverse %}
  {% for review in reviews %}
  	{% include book-review.html %}
  {% endfor %}

 </div>
