---
layout: page
title: Latest posts
---

<hr>

<ul>
  {% for post in site.posts %}
    <style="fontsize:10vw">
    <li>
      <a href="{{ post.url }}" style="fontsize:10vw">
        {{ post.title }}
      </a>
      - <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    </li>
    <br>
  {% endfor %}
</ul>