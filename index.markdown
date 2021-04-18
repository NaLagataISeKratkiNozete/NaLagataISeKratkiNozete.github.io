---
layout: default
---

<div class="posts">
  {% for post in site.posts %}
  <ul> 
    {% if post.excerpt %}
    <article class="post">
      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>

      <div class="entry">
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Прочитај повеќе</a>
    </article>
    {% endif %}
  </ul>
  {% endfor %}
</div>