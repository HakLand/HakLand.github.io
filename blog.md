---
layout: default
title: Blog
description: 
---

{% for post in site.posts %}
<div class="tool">
    <a href="post.url">
    <img class="tool-pic" src="{{ post.main_image }}"/>
    <div class="tool-description">
        <h3 class="tool-title">{{ post.title }}</h3>
        <p>
            {{ post.description }}
        </p>
    </div>
    </a>
</div>
{% endfor %}
