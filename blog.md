---
layout: default
title: Blog
description: 
---

<div class="posts">
  {% for post in site.posts %}
  <div class="post">
      <h1 class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></h1>
      <a href="{{ post.url }}"><img src="{{post.main_image}}" style="border: 1px solid #000; max-width:128px; max-height:128px;">></a>
      <h2 class="post-description">{{ post.description }}<span style="font-weight:100;font-size:  0.7em;"> by {{post.author}}</span></h2>
      <span class="post-date">{{ post.date | date_to_string }}</span>
    </div>
  {% endfor %}
</div>
