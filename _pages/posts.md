---
title: "Posts"
permalink: /posts/
layout: single
author_profile: true
---

시리즈로 묶이지 않는 단발성 포스트를 모아둡니다.

---

{% assign post_list = site.posts | where_exp: "post", "post.categories contains 'posts'" %}
{% if post_list.size > 0 %}
{% for post in post_list %}
- [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%Y-%m-%d" }}
{% endfor %}
{% else %}
*아직 작성된 포스트가 없습니다. 곧 올라옵니다!*
{% endif %}
