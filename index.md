---
layout: default
title: Top Page
---

<main>
  <h3>POSTS</h3>
  {% for post in site.posts %}
    <aside>
      <h3>
        <span>{{ post.date | date: "%b %d, %y"}}</span>
        <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
      </h3>
    </aside>  
  {% endfor %}
</main>