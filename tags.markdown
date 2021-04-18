---
layout: page
title: Тагови
permalink: /tags/
---

<div class="posts">
  {% for category in site.categories %}
  <h1>{{ category | first }}</h1>
  <ul>
    {% for posts in category %}
    {% for post in posts %}
    {% if post.excerpt %}
    <article class="post">
      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>
      <div class="entry">
        {{ post.excerpt }}
      </div>
    </article>
    {% endif %}
    {% endfor %}
    {% endfor %}
  </ul>
  {% endfor %}
</div>