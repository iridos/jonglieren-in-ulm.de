---
layout: default
title: Jonglieren in Ulm
---

<div>
{% for post in site.posts %}
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>

    <p>{{ post.content }}</p>
    <p class="signatur">{{ post.author }} - {{ post.date| date: "%d.%m.%Y" }}</p>
{% endfor %}
</div>
