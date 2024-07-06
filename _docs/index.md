---
---
{% assign docs = site.docs %}

{% for doc in docs %}
    <p><a href="{{doc.url}}">{{doc.title}}</href></p>
{% endfor %}