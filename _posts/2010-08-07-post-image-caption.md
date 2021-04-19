---
title: "Post: Image (Caption)"
categories: [minimal-mistakes]
hidden: true
  - Post Formats
tags:
  - image
  - Post Formats
---

{% capture fig_img %}
![Foo]({{ "/assets/images/unsplash-gallery-image-3.jpg" | relative_url }})
{% endcapture %}

<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>Photo from Unsplash.</figcaption>
</figure>
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTgxNDU1MTYyM119
-->