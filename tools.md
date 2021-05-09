---
layout: default
title: Hackland Tools
description: Tools at Hackland
---

<h1>Hackland Tools</h1>

Click on a tool for more info.

<ul>
{% for post in site.posts %}
{% if post.categories contains "tools" %}
    <li><a href="#{{ post.id }}">{{ post.title }}</a></li>
{% endif %}
{% endfor %}
</ul>

<!--
{% for post in site.posts %}
{% if post.categories contains "tools" %}
<div class="tool">
    <a href="{{ post.url }}"><img class="tool-pic" src="{{ post.main_image }}" id="{{ post.id }}"/></a>
    <div class="tool-description">
        <a href="{{ post.url }}"><h3 class="tool-title">{{ post.title }}</h3></a>
        <p>
            {{ post.description }}
        </p>
    </div>
</div>
{% endif %}
{% endfor %}
-->
