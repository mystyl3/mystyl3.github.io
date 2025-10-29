---
layout: default
title: "Beranda"
description: "Selamat datang di blog Wildan Hidayat — berbagi cerita, ide, dan pengalaman menarik."
---
<h1>{{ site.title }}</h1>
<p>{{ site.description }}</p>

<div class="posts">
  {% for post in site.posts %}
    <article>
      <a href="{{ post.url }}">
        {% if post.thumbnail %}
          <img src="{{ post.thumbnail }}" alt="{{ post.title }}">
        {% endif %}
        <h2>{{ post.title }}</h2>
        <p>{{ post.description }}</p>
      </a>
    </article>
  {% endfor %}
</div>
