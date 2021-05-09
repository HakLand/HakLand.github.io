---
layout: default
title: Blog
description: 
---

{% for post in site.posts %}
<div class="tool">
    <a href="{{ post.url }}"><img class="tool-pic" src="{{ post.main_image }}"/></a>
    <div class="tool-description">
        <a href="{{ post.url }}"><h3 class="tool-title">{{ post.title }}</h3></a>
        <p>
            {{ post.description }}
        </p>
    </div>
</div>
{% endfor %}
