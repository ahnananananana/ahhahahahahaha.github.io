---
layout: default
title: Home
---

<h1>블로그 목록</h1>
<ul>
  {% for post in paginator.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> <span>({{ post.date | date: "%Y-%m-%d" }})</span>
    </li>
  {% endfor %}
</ul>
