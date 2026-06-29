---
layout: default
title: "Блог"
permalink: /blog/
---

<h1>Все записи</h1>
<div class="journal-list">
  {% for post in site.posts %}
    <div class="item">
      <a href="{{ post.url }}">{{ post.title }}</a>
      — {{ post.date | date: "%d.%m.%Y" }}
    </div>
  {% endfor %}
</div>

<article class="post">
    <header class="post-header">
        <h1>{{ page.title }}</h1>
        <p class="post-meta">{{ page.date | date: "%b %d %Y, %I:%M%P" }}</p>
    </header>

    <div class="post-content">
        {{ content }}
    </div>

    <div class="item">
    {{ content }}
    </div>

    <footer class="post-footer">
        <p><a href="/blog/">← Назад к списку</a></p>
    </footer>
</article>
