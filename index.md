---
layout: home
image: assets/image/banner/home.jpg
---

{% for post in site.posts %}

{{ post.date | date_to_string }} » {{ post.title }}
{% endfor %}