---
layout: home
image: assets/image/banner/home.jpg
---

{% for post in site.posts %}

{{ post.title }}
{% endfor %}