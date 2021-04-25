---
layout: page
title: Latest posts
---

<hr>

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">
        fontsize: 40px;
        {{ post.title }}
      </a>
      - <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    </li>
    <br>
  {% endfor %}
</ul>