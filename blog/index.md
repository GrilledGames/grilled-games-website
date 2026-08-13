---
layout: default
title: Blog — Grilled Games
permalink: /blog/
---

# Blog

News, updates, and stories from the Grilled Games studio.

<div class="post-list">
  {% for post in site.posts %}
    <article>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <time datetime="{{ post.date | date_to_iso }}">{{ post.date | date: "%B %d, %Y" }}</time>
      {{ post.excerpt }}
    </article>
  {% endfor %}
</div>

{% if site.posts.size == 0 %}
<p>No posts yet. Check back soon!</p>
{% endif %}
