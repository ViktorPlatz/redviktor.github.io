---
layout: page
title: Latest posts
---

<hr>

{% if node.layout == "post" %}
  <article>
    <h2>
      <a href="{{ node.url }}">
        {{ node.title }}
      </a>
    </h2>
    <time datetime="{{ node.date | date: "%Y-%m-%d" }}">{{ site.date | date_to_long_string }}</time>
    {{ node.content }}
  </article>
{% endif %}