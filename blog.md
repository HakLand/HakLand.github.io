---
layout: default
title: Blog
description: 
pagination: 
  enabled: true
---

<div class="posts">
  {% for post in site.posts %}
    <div class="post">
      <h1 class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></h1>
      <h2 class="post-description">{{ post.description }}<span style="font-weight:100;font-size:  0.7em;"> by {{post.author}}</span></h2>
      <span class="post-date">{{ post.date | date_to_string }}</span>
    </div>
  {% endfor %}
</div>
