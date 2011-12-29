---
layout: default
title: Jonglieren in Ulm
---

<div>
{% for post in site.posts %}
    <p><a href="{{ post.url }}">{{ post.title }}</a></p>

    <p>{{ post.content | strip_html | truncatewords: 32 }} <a href="{{ post.url }}">mehr</a></p>
{% endfor %}
</div>
