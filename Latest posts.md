---
layout: page
title: Latest posts
---

<hr>

{% if node.layout == "post" %}
  <article>
    <h2>
      <a href="{{ "/" | relative_url }}">
        {{ post.title }}
      </a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    {{ post.content }}
  </article>
{% endif %}