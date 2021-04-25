---
layout: page
title: Latest posts
---

<hr>

{% if node.layout == "post" %}
  <article>
    <h2>
      <a href="{{ page.url }}">
        {{ node.title }}
      </a>
    </h2>
    <time datetime="{{ page.date | date: "%Y-%m-%d" }}">{{ page.date | date_to_long_string }}</time>
    {{ page.content }}
  </article>
{% endif %}