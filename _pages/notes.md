---
title: "Notes"
permalink: /notes/
layout: single
author_profile: true
---

강의 노트, 공부 정리, 그리고 물리학 관련 메모를 모아둡니다.

---

{% assign notes_posts = site.posts | where_exp: "post", "post.categories contains 'notes'" %}
{% if notes_posts.size > 0 %}
{% for post in notes_posts %}
- [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%Y-%m-%d" }}
{% endfor %}
{% else %}
*아직 작성된 노트가 없습니다. 곧 올라옵니다!*
{% endif %}
