---
title: "Notes"
permalink: /notes/
layout: single
author_profile: true
---

연구하면서 공부한 내용을 정리합니다.

---

{% assign notes_posts = site.posts | where_exp: "post", "post.categories contains 'notes'" %}
{% if notes_posts.size > 0 %}
{% for post in notes_posts %}
- [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%Y-%m-%d" }}
{% endfor %}
{% else %}
*아직 작성된 노트가 없습니다. 곧 올라옵니다!*
{% endif %}
