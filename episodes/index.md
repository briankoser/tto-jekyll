---
title: Episodes
layout: default
description: The podcast where we make top ten lists about everything!
---
# Episodes

{% for post in site.posts %}
<article>
    <header>
        <h2 class="post-title"><a href="/{{ post.url }}">#{{ post.number }}: {{ post.title | escape }}</a></h2>
        <span class="post-date">
            <svg class="icon icon-calendar"><use xlink:href="#icon-calendar"></use></svg>
            {{ post.pub_date }}
        </span>
        <span class="post-comments">
            <svg class="icon icon-bubble"><use xlink:href="#icon-bubble"></use></svg>
            <a href="/{{ post.url }}#disqus_thread">Comments</a>
        </span>
    </header>
</article>
{% endfor %}