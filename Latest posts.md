---
layout: page
title: Latest posts
---

<hr>

<ul>
  {% for post in site.posts %}
    <li>
      fontsize:40px;
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
      - <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    </li>
    <br>
  {% endfor %}
</ul>