---
layout: page
title: Latest posts
---

<hr>



<ul style="list-style-type:none">
  {% for post in site.posts %}
    <li style="font-size:20px">
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
      - <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    </li>
    <br>
  {% endfor %}
</ul>