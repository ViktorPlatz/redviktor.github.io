---
layout: page
title: Latest posts
---

<hr>

{% if node.layout == "post" %}
  <article>
    <h2>
      <a href="{{ site.url }}">
        {{ site.title }}
      </a>
    </h2>
    <time datetime="{{ site.date | date: "%Y-%m-%d" }}">{{ site.date | date_to_long_string }}</time>
    {{ site.content }}
  </article>
{% endif %}