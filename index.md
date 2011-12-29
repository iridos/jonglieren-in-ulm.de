---
layout: default
title: Jonglieren in Ulm
---

<h1>{{ page.title }}</h1>

<div>
{% for post in site.posts %}
    <p style="font-size: large">{{ post.date|date:"%d.%m.%Y" }}: <a href="{{ post.url }}">{{ post.title }}</a></p>

    <p>{{ post.content | strip_html | truncatewords: 32 }} <a href="{{ post.url }}">mehr</a></p>
{% endfor %}
</div>
