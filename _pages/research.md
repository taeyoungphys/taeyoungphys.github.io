---
title: "Research"
permalink: /research/
layout: single
author_profile: true
---

전산다체물리 연구와 관련된 노트를 정리합니다.

### 주요 주제

- **텐서 네트워크 (Tensor Networks)** — MPS, DMRG, TEBD 등
- **FTNO** — 연구 진행 중인 프로젝트 노트
- **수치 계산 방법론** — Julia 기반 구현 및 벤치마크

---

*연구 노트가 올라오면 아래에 목록이 추가됩니다.*

{% assign research_posts = site.posts | where_exp: "post", "post.categories contains 'research'" %}
{% for post in research_posts %}
- [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%Y-%m-%d" }}
{% endfor %}
